# VTP


- If the vtp domain is NULL it will be set on arive of the first VTP packet.
- VTPv1 Server/Client change to v2 if he recieve a v2 packet when v1 is not explicit configured



## VTP v1
### Summarz Advertisement
```
Frame 1350: 99 bytes on wire (792 bits), 99 bytes captured (792 bits) on interface 0
IEEE 802.3 Ethernet 
    Destination: CDP/VTP/DTP/PAgP/UDLD (01:00:0c:cc:cc:cc)
    Source: CiscoInc_27:d1:02 (68:bd:ab:27:d1:02)
    Length: 85
Logical-Link Control
VLAN Trunking Protocol
    Version: 0x01
    Code: Summary Advertisement (0x01)
    Followers: 1
    Management Domain Length: 3
    Management Domain: lab
    Configuration Revision Number: 4
    Updater Identity: 0.0.0.0
    Update Timestamp: 93-03-01 00:16:54
    MD5 Digest: 468537c1da57e079b167ca068eb281c4

```

### Subset Advertisement
```
Frame 1351: 286 bytes on wire (2288 bits), 286 bytes captured (2288 bits) on interface 0
IEEE 802.3 Ethernet 
    Destination: CDP/VTP/DTP/PAgP/UDLD (01:00:0c:cc:cc:cc)
    Source: CiscoInc_27:d1:02 (68:bd:ab:27:d1:02)
    Length: 272
Logical-Link Control
VLAN Trunking Protocol
    Version: 0x01
    Code: Subset Advertisement (0x02)
    Sequence Number: 1
    Management Domain Length: 3
    Management Domain: lab
    Configuration Revision Number: 4
    VLAN Information
    VLAN Information
    VLAN Information
    VLAN Information
        VLAN Information Length: 20
        Status: 0x00
        VLAN Type: Ethernet (0x01)
        VLAN Name Length: 5
        ISL VLAN ID: 0x000c
        MTU Size: 1500
        802.10 Index: 0x000186ac
        VLAN Name: lab12
    VLAN Information
    VLAN Information
    VLAN Information
    VLAN Information
```

- ***only standard vlans allowed (1-1005) on device***



## VTP v2
### Summarz Advertisement
```
Frame 33: 102 bytes on wire (816 bits), 102 bytes captured (816 bits) on interface 0
IEEE 802.3 Ethernet 
    Destination: CDP/VTP/DTP/PAgP/UDLD (01:00:0c:cc:cc:cc)
    Source: CiscoInc_27:d1:02 (68:bd:ab:27:d1:02)
    Length: 88
Logical-Link Control
VLAN Trunking Protocol
    Version: 0x02
    Code: Summary Advertisement (0x01)
    Followers: 1
    Management Domain Length: 3
    Management Domain: lab
    Configuration Revision Number: 5
    Updater Identity: 0.0.0.0
    Update Timestamp: 93-03-01 00:27:10
    MD5 Digest: 4ed79f393ac5af51382e05ef48d85d73
```

### Subset Advertisement
```
Frame 34: 282 bytes on wire (2256 bits), 282 bytes captured (2256 bits) on interface 0
IEEE 802.3 Ethernet 
    Destination: CDP/VTP/DTP/PAgP/UDLD (01:00:0c:cc:cc:cc)
    Source: CiscoInc_27:d1:02 (68:bd:ab:27:d1:02)
    Length: 268
Logical-Link Control
VLAN Trunking Protocol
    Version: 0x02
    Code: Subset Advertisement (0x02)
    Sequence Number: 1
    Management Domain Length: 3
    Management Domain: lab
    Configuration Revision Number: 5
    VLAN Information
    VLAN Information
    VLAN Information
    VLAN Information
        VLAN Information Length: 20
        Status: 0x00
        VLAN Type: Ethernet (0x01)
        VLAN Name Length: 5
        ISL VLAN ID: 0x000c
        MTU Size: 1500
        802.10 Index: 0x000186ac
        VLAN Name: lab12
    VLAN Information
    VLAN Information
    VLAN Information
    VLAN Information
```

- ***only standard vlans allowed (1-1005) on device***

## VTP v3
Mode (Server / Client / Transparent) for (MST / VLAN / unknown VTP instances)

You have to chose your primary server

```
Switch#vtp primary
This system is becoming primary server for feature vlan
No conflicting VTP3 devices found.
Do you want to continue? [confirm]
```

> Switch(config)#vlan 21
> VTP VLAN configuration not allowed when device is not the primary server for vlan database.




## Verivication
```
Switch#show vtp status
VTP Version capable             : 1 to 3
VTP version running             : 3
VTP Domain Name                 : lab
VTP Pruning Mode                : Disabled
VTP Traps Generation            : Disabled
Device ID                       : 68bd.ab27.d100

Feature VLAN:
--------------
VTP Operating Mode                : Primary Server
Number of existing VLANs          : 11
Number of existing extended VLANs : 2
Configuration Revision            : 2
Primary ID                        : 68bd.ab27.d100
Primary Description               : Switch
MD5 digest                        : 0x1D 0x86 0x48 0x25 0x61 0xD1 0x8C 0x34
                                    0xED 0x0E 0x91 0x62 0xD1 0xA2 0x10 0x0C


Feature MST:
--------------
VTP Operating Mode                : Transparent


Feature UNKNOWN:
--------------
VTP Operating Mode                : Transparent
```


## VTP Pruning
VTP pruning eliminates the need to statically remove VLANs from the allowed trunking list of a port by having the switches automatically communicate to each other which VLANs they have locally assigned or are in the transit path for. The `show interface pruning` command indicates what traffic the local switch told its neighbor that it needs, via the VLAN traffic requested of neighbor field. These VLANs are either locally assigned to certain ports, or those for which the local switch is in the Layer 2 transit path and traffic was requested by neighbor switches. The Vlans pruned for lack of request by neighbor field indicates the VLANs that the upstream neighbor did not request. ***VTP pruning can be enabled only on the device running in server mode***, and the settings will be inherited by all devices in the same VTP domain.