# Assigning the Switch IP Address and Default Gateway
> This chapter describes how to create the initial switch configuration (for example, assigning the IP address and default gateway information) for the Catalyst 3560 switch by using a variety of automatic and manual methods. It also describes how to modify the switch startup configuration.
> For IP Version 6 (IPv6) see Chapter “Configuring IPv6 Unicast Routing”. **To enable IPv6, the switch must be running the IP services image.**
## Understanding the Boot Process
Normal boot process involves the operation of the boot loader software
- low-level CPU initialization
- power-on self-test (POST)
- loads a default operating system software image into memory and boots up the switch.

> The boot loader also provides trap-door access into the system if the operating system has problems serious enough that it cannot be used. (**ROMON**)


## Assigning Switch Information
- Default switch console port settings
  - Baud rate: 9600
  - Data bits: 8
  - Stop bits: 1
  - Parity: none

> You can assign IP information through the switch setup program, through a DHCP server, or manually.

> If you are using DHCP, do not respond to any of the questions in the setup program until the switch receives the dynamically assigned IP address and reads the configuration file.

- Default Switch Information
  - IP address and subnet mask
    - No IP address or subnet mask are defined.
  - Default gateway
    - No default gateway is defined.
  - Enable secret password
    - No password is defined.
  - Hostname
    - The factory-assigned default hostname is *Switch*.
  - Telnet password
    - No password is defined.
  - Cluster command switch functionality
    - Disabled.
  - Cluster name
    - No cluster name is defined.

### Understanding DHCP-Based Autoconfiguration
- DHCP Client Request Process
  - When you boot up your switch, the DHCP client is invoked and requests configuration information from a DHCP server when the configuration file is not present on the switch. `ip address dhcp` on a routed interfaces invokes the DHCP client manually.
- Autoconfiguration
  - The downloaded configuration file becomes the running configuration of the switch. It does not over write the bootup configuration saved in the flash.
  - Downloaded configuration is appended. Any existing configuration is not overwritten.
- Auto-Image Update
  - DHCP auto-image upgrade with DHCP autoconfiguration to download both a configuration and a new image.
- Limitations and Restrictions
  - at least one Layer 3 interface in an up state without a static assigned IP address
  - per default the switch tries indefinitelz to download an IP address.
  - stops if a configuration file cannot be downloaded

- DHCP Options  
  - 67
    - configuration filename
  - 66
    - DHCP server hostname
  - 150
    - TFTP server address
  - 125
    - description of the file
	- Specify the path to the text file that describes the path to the image file.

> If the router IP address or the TFTP server name are not found, the switch might send broadcast, instead of unicast, TFTP requests. (255.255.255.255)
> If the configuration file could not be downloaded, the switch attempts to download a configuration file by using various combinations of filenames and TFTP server addresses. The files include the specified configuration filename (if any) and these files: network-config, cisconet.cfg, *hostname*.config, or *hostname*.cfg.
- TFTP files
  - The configuration file named in the DHCP reply (the actual switch configuration file).
  - The network-confg or the cisconet.cfg file (known as the default configuration files).
  - The router-confg or the ciscortr.cfg file (These files contain commands common to all switches. Normally, if the DHCP and TFTP servers are properly configured, these files are not accessed.)	

- Configuring the Relay Device
  - `router(config-if)# ip helper-address 20.0.0.2`
  

#### Obtaining Configuration Files
- The IP address and the configuration filename is reserved for the switch and provided in the DHCP reply
  -  The switch sends a unicast message to the TFTP server to retrieve the named configuration file from the base directory of the server and upon receipt, it completes its boot-up process.
- The IP address and the configuration filename is reserved for the switch, but the TFTP server address is not provided in the DHCP reply
  - The switch sends a broadcast message to a TFTP server to retrieve the named configuration file from the base directory of the server, and upon receipt, it completes its boot-up process.
- Only the IP address is reserved for the switch and provided in the DHCP reply. The configuration filename is not provided
  - The switch receives its IP address, subnet mask, and the TFTP server address from the DHCP server. The switch sends a unicast message to the TFTP server to retrieve the network-confg or cisconet.cfg default configuration file. (If the network-confg file cannot be read, the switch reads the cisconet.cfg file.)
  - The default configuration file contains the hostnames-to-IP-address mapping for the switch. The switch fills its host table with the information in the file and obtains its hostname. If the hostname is not found in the file, the switch uses the hostname in the DHCP reply. If the hostname is not specified in the DHCP reply, the switch uses the default Switch as its hostname.
  - After obtaining its hostname from the default configuration file or the DHCP reply, the switch reads the configuration file that has the same name as its hostname ( hostname -confg or hostname.cfg, depending on whether network-confg or cisconet.cfg was read earlier) from the TFTP server. If the cisconet.cfg file is read, the filename of the host is truncated to eight characters.
  - If the switch cannot read the network-confg, cisconet.cfg, or the hostname file, it reads the router-confg file. If the switch cannot read the router-confg file, it reads the ciscortr.cfg file.
  


#### Example Configuration
Configure a switch as a DHCP server so that it will download a configuration file.
```
Switch# configure terminal
Switch(config)# ip dhcp pool pool1
Switch(dhcp-config)# network 10.10.10.0 255.255.255.0
Switch(dhcp-config)# bootfile config-boot.text
Switch(dhcp-config)# default-router 10.10.10.1
Switch(dhcp-config)# option 150 10.10.10.1
Switch(dhcp-config)# exit
Switch(config)# tftp-server flash:config-boot.text
Switch(config)# interface gigabitethernet0/4
Switch(config-if)# no switchport
Switch(config-if)# ip address 10.10.10.1 255.255.255.0
Switch(config-if)# end
```

This example shows how to configure a switch as a DHCP server so it downloads a configuration file:

> Before following the steps in this table, you **must create a text file** (for example, autoinstall_dhcp) that will be uploaded to the switch. In the text file, put the **name of the image** that you want to download. This **image must be a tar** and not a bin file.
```
Switch# config terminal
Switch(config)# ip dhcp pool pool1
Switch(dhcp-config)# network 10.10.10.0 255.255.255.0
Switch(dhcp-config)# bootfile config-boot.text
Switch(dhcp-config)# default-router 10.10.10.1
Switch(dhcp-config)# option 150 10.10.10.1
Switch(dhcp-config)# option 125 hex 0000.0009.0a05.08661.7574.6f69.6e73.7461.6c6c.5f64.686370
Switch(dhcp-config)# exit
Switch(config)# tftp-server flash:config-boot.text
Switch(config)# tftp-server flash:c3560-ipservices-mz.122-44.3.SE.tar
Switch(config)# tftp-server flash:boot-config.text
Switch(config)# tftp-server flash: autoinstall_dhcp
Switch(config)# interface gigabitethernet0/4
Switch(config-if)# no switchport
Switch(config-if)# ip address 10.10.10.1 255.255.255.0
Switch(config-if)# end
```

#### Configuring the Client
- Enable autoconfiguration with a saved configuration.
  - `Switch(config)# boot host dhcp`
- (Optional) Set the amount of time the system tries to download a configuration file. Default: indefinitely
  - `Switch(config)# boot host retry timeout <60-65535>`

```
Switch# configure terminal
Switch(conf)# boot host dhcp
Switch(conf)# boot host retry timeout 300
Switch(conf)# banner config-save ^C Caution - Saving Configuration File to NVRAM May Cause You to No longer Automatically Download Configuration Files at Reboot^C
Switch(config)# vlan 99
Switch(config-vlan)# interface vlan 99
Switch(config-if)# no shutdown
Switch(config-if)# end
Switch# show boot
BOOT path-list:
Config file: flash:/config.text
Private Config file: flash:/private-config.text
Enable Break: no
Manual Boot: no
HELPER path-list:
NVRAM/Config file
buffer size: 32768
Timeout for Config
Download: 300 seconds
Config Download
via DHCP: enabled (next boot: enabled)
Switch#
```

### Manually Assigning IP Information

## Checking and Saving the Running Configuration

### Configuring the NVRAM Buffer Size

## Modifying the Startup Configuration

### Default Boot Configuration
### Automatically Downloading a Configuration File
### Specifying the Filename to Read and Write the System Configuration
### Booting Manually
### Booting a Specific Software Image
### Controlling Environment Variables

## Scheduling a Reload of the Software Image

### Configuring a Scheduled Reload
### Displaying Scheduled Reload Information

## Boot Loader Upgrade and Image Verification for the FIPS Mode of Operation