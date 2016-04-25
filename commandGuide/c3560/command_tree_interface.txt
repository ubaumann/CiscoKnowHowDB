# interface Fa 0/1

## switchport ?

+ access
  + Set access mode characteristics of the interface
  + vlan
    + Set VLAN when interface is in access mode
    + <1-4094>
      + VLAN ID of the VLAN when this port is in access mode
        + <cr>
    + dynamic
      + When in access mode, this interfaces VLAN is controlled by VMPS
        + <cr>
+ autostate
  + Include or exclude this port from vlan link up calculation
  + exclude
    + Exclude this port from vlan link up calculation
      + <cr>
+ backup
  + Set backup for the interface
  + interface
    + Specify an interface as backup
    + FastEthernet
      + FastEthernet IEEE 802.3
      + <0-0>
        + FastEthernet interface number
        + mmu
          + mac-address move update
          + primary
            + mac-address move update primary vlan
            + vlan
              + mac-address move update primary vlan
              + <1-4094>
                + vlan id
                  + <cr>
        + multicast
          + multicast parameters
          + fast-convergence
            + configure fast convergence on backup interface
              + <cr>
        + preemption
          + preemption parameters
          + delay
            + preemption parameters
            + <1-300>
              + preemption delay in seconds
                + <cr>
          + mode
            + set the preemption mode
            + bandwidth
              + higher bandwidth interface preferred
                + <cr>
            + forced
              + active interface preferred
                + <cr>
            + off
              + turn off preemption
                + <cr>
        + prefer
          + load-balancing
          + vlan
            + Preferred vlans on the backup interface for load-balancing
            + WORD
              + VLAN IDs 1-4094
                + <cr>
          + <cr>
    + GigabitEthernet
      + GigabitEthernet IEEE 802.3z
      + <0-0>
        + GigabitEthernet interface number
        + mmu
          + mac-address move update
          + primary
            + mac-address move update primary vlan
            + vlan
              + mac-address move update primary vlan
              + <1-4094>
                + vlan id
                  + <cr>
        + multicast
          + multicast parameters
          + fast-convergence
            + configure fast convergence on backup interface
              + <cr>
        + preemption
          + preemption parameters
          + delay
            + preemption parameters
            + <1-300>
              + preemption delay in seconds
                + <cr>
          + mode
            + set the preemption mode
            + bandwidth
              + higher bandwidth interface preferred
                + <cr>
            + forced
              + active interface preferred
                + <cr>
            + off
              + turn off preemption
                + <cr>
        + prefer
          + load-balancing
          + vlan
            + Preferred vlans on the backup interface for load-balancing
            + WORD
              + VLAN IDs 1-4094
                + <cr>
          + <cr>
    + Port-channel
      + Ethernet Channel of interfaces
      + <1-48>
        + Port-channel interface number
        + mmu
          + mac-address move update
          + primary
            + mac-address move update primary vlan
            + vlan
              + mac-address move update primary vlan
              + <1-4094>
                + vlan id
                  + <cr>
        + multicast
          + multicast parameters
          + fast-convergence
            + configure fast convergence on backup interface
              + <cr>
        + preemption
          + preemption parameters
          + delay
            + preemption parameters
            + <1-300>
              + preemption delay in seconds
                + <cr>
          + mode
            + set the preemption mode
            + bandwidth
              + higher bandwidth interface preferred
                + <cr>
            + forced
              + active interface preferred
                + <cr>
            + off
              + turn off preemption
                + <cr>
        + prefer
          + load-balancing
          + vlan
            + Preferred vlans on the backup interface for load-balancing
            + WORD
              + VLAN IDs 1-4094
                + <cr>
          + <cr>
+ block
  + Disable forwarding of unknown uni/multi cast addresses
  + multicast
    + Block unknown multicast addresses
      + <cr>
  + unicast
    + Block unknown unicast addresses
      + <cr>
+ host
  + Set port host
    + <cr>
+ mode
  + Set trunking mode of the interface
  + access
    + Set trunking mode to ACCESS unconditionally
      + <cr>
  + dot1q-tunnel
    + set trunking mode to TUNNEL unconditionally
      + <cr>
  + dynamic
    + Set trunking mode to dynamically negotiate access or trunk mode
    + auto
      + Set trunking mode dynamic negotiation parameter to AUTO
        + <cr>
    + desirable
      + Set trunking mode dynamic negotiation parameter to DESIRABLE
        + <cr>
  + private-vlan
    + Set private-vlan mode
    + host
      + Set the mode to private-vlan host
        + <cr>
    + promiscuous
      + Set the mode to private-vlan promiscuous
        + <cr>
  + trunk
    + Set trunking mode to TRUNK unconditionally
      + <cr>
+ nonegotiate
  + Device will not engage in negotiation protocol on this interface
    + <cr>
+ port-security
  + Security related command
  + aging
    + Port-security aging commands
    + static
      + Enable aging for configured secure addresses
        + <cr>
    + time
      + Port-security aging time
      + <1-1440>
        + Aging time in minutes. Enter a value between 1 and 1440
          + <cr>
    + type
      + Port-security aging type
      + absolute
        + Absolute aging (default)
          + <cr>
      + inactivity
        + Aging based on inactivity time period
          + <cr>
  + mac-address
    + Secure mac address
    + H.H.H
      + 48 bit mac address
        + <cr>
    + sticky
      + Configure dynamic secure addresses as sticky
        + <cr>
  + maximum
    + Max secure addresses
    + <1-1536>
      + Maximum addresses
        + <cr>
  + violation
    + Security violation mode
    + protect
      + Security violation protect mode
        + <cr>
    + restrict
      + Security violation restrict mode
        + <cr>
    + shutdown
      + Security violation shutdown mode
      + vlan
        + Security violation shutdown vlan mode
          + <cr>
        + <cr>
    + <cr>
+ priority
  + Set appliance 802.1p priority
  + extend
    + Set appliance 802.1p priority
    + cos
      + Override 802.1p priority of devices on appliance
      + <0-7>
        + Priority for devices on appliance
          + <cr>
    + trust
      + Trust 802.1p priorities of devices on appliance
        + <cr>
+ private-vlan
  + Set the private VLAN configuration
  + association
    + Set the private VLAN association
    + host
      + Set the private VLAN host association
      + <1006-4094>
        + Primary extended range VLAN ID of the private VLAN host port association
        + <1006-4094>
          + Secondary extended range VLAN ID of the private VLAN host port association
            + <cr>
        + <2-1001>
          + Secondary normal range VLAN ID of the private VLAN host port association
            + <cr>
      + <2-1001>
        + Primary normal range VLAN ID of the private VLAN port association
        + <1006-4094>
          + Secondary extended range VLAN ID of the private VLAN host port association
            + <cr>
        + <2-1001>
          + Secondary normal range VLAN ID of the private VLAN host port association
            + <cr>
    + mapping
      + Set the private VLAN promiscuous mapping
      + <1006-4094>
        + Primary extended range VLAN ID of the private VLAN promiscuous port mapping
        + WORD
          + Secondary VLAN IDs of the private VLAN promiscuous port mapping
            + <cr>
        + add
          + Add a VLAN to private VLAN list
          + WORD
            + Secondary VLAN IDs of the private VLAN promiscuous port mapping
              + <cr>
        + remove
          + Remove a VLAN from private VLAN list
          + WORD
            + Secondary VLAN IDs of the private VLAN promiscuous port mapping
              + <cr>
      + <2-1001>
        + Primary normal range VLAN ID of the private VLAN promiscuous port mapping
        + WORD
          + Secondary VLAN IDs of the private VLAN promiscuous port mapping
            + <cr>
        + add
          + Add a VLAN to private VLAN list
          + WORD
            + Secondary VLAN IDs of the private VLAN promiscuous port mapping
              + <cr>
        + remove
          + Remove a VLAN from private VLAN list
          + WORD
            + Secondary VLAN IDs of the private VLAN promiscuous port mapping
              + <cr>
  + host-association
    + Set the private VLAN host association
    + <1006-4094>
      + Primary extended range VLAN ID of the private VLAN host port association
      + <1006-4094>
        + Secondary extended range VLAN ID of the private VLAN host port association
          + <cr>
      + <2-1001>
        + Secondary normal range VLAN ID of the private VLAN host port association
          + <cr>
    + <2-1001>
      + Primary normal range VLAN ID of the private VLAN port association
      + <1006-4094>
        + Secondary extended range VLAN ID of the private VLAN host port association
          + <cr>
      + <2-1001>
        + Secondary normal range VLAN ID of the private VLAN host port association
          + <cr>
  + mapping
    + Set the private VLAN promiscuous mapping
    + <1006-4094>
      + Primary extended range VLAN ID of the private VLAN promiscuous port mapping
      + WORD
        + Secondary VLAN IDs of the private VLAN promiscuous port mapping
          + <cr>
      + add
        + Add a VLAN to private VLAN list
        + WORD
          + Secondary VLAN IDs of the private VLAN promiscuous port mapping
            + <cr>
      + remove
        + Remove a VLAN from private VLAN list
        + WORD
          + Secondary VLAN IDs of the private VLAN promiscuous port mapping
            + <cr>
    + <2-1001>
      + Primary normal range VLAN ID of the private VLAN promiscuous port mapping
      + WORD
        + Secondary VLAN IDs of the private VLAN promiscuous port mapping
          + <cr>
      + add
        + Add a VLAN to private VLAN list
        + WORD
          + Secondary VLAN IDs of the private VLAN promiscuous port mapping
            + <cr>
      + remove
        + Remove a VLAN from private VLAN list
        + WORD
          + Secondary VLAN IDs of the private VLAN promiscuous port mapping
            + <cr>
+ protected
  + Configure an interface to be a protected port
    + <cr>
+ trunk
  + Set trunking characteristics of the interface
  + allowed
    + Set allowed VLAN characteristics when interface is in trunking mode
    + vlan
      + Set allowed VLANs when interface is in trunking mode
      + WORD
        + VLAN IDs of the allowed VLANs when this port is in trunking mode
          + <cr>
      + add
        + add VLANs to the current list
        + WORD
          + VLAN IDs of the allowed VLANs when this port is in trunking mode
            + <cr>
      + all
        + all VLANs
          + <cr>
      + except
        + all VLANs except the following
        + WORD
          + VLAN IDs of disallowed VLANS when this port is in trunking mode
            + <cr>
      + none
        + no VLANs
          + <cr>
      + remove
        + remove VLANs from the current list
        + WORD
          + VLAN IDs of disallowed VLANS when this port is in trunking mode
            + <cr>
  + encapsulation
    + Set trunking encapsulation when interface is in trunking mode
    + dot1q
      + Interface uses only 802.1q trunking encapsulation when trunking
        + <cr>
    + isl
      + Interface uses only ISL trunking encapsulation when trunking
        + <cr>
    + negotiate
      + Device will negotiate trunking encapsulation with peer on interface
        + <cr>
  + native
    + Set trunking native characteristics when interface is in trunking mode
    + vlan
      + Set native VLAN when interface is in trunking mode
      + <1-4094>
        + VLAN ID of the native VLAN when this port is in trunking mode
          + <cr>
  + pruning
    + Set pruning VLAN characteristics when interface is in trunking mode
    + vlan
      + Set VLANs enabled for pruning when interface is in trunking mode
      + WORD
        + VLAN IDs of the allowed VLANs when this port is in trunking mode
          + <cr>
      + add
        + add VLANs to the current list
        + WORD
          + VLAN IDs of the allowed VLANs when this port is in trunking mode
            + <cr>
      + except
        + all VLANs except the following
        + WORD
          + VLAN IDs of disallowed VLANS when this port is in trunking mode
            + <cr>
      + none
        + no VLANs
          + <cr>
      + remove
        + remove VLANs from the current list
        + WORD
          + VLAN IDs of disallowed VLANS when this port is in trunking mode
            + <cr>
+ voice
  + Voice appliance attributes
  + vlan
    + Vlan for voice traffic
    + <1-4094>
      + Vlan for voice traffic
        + <cr>
    + dot1p
      + Priority tagged on PVID
        + <cr>
    + none
      + Don't tell telephone about voice vlan
        + <cr>
    + untagged
      + Untagged on PVID
        + <cr>
  + <cr>