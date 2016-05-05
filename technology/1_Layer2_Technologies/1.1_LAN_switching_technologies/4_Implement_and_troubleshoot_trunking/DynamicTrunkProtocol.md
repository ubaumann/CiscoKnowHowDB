# Dynamic Trunk Protocol

## Packet
Frame 1: 60 bytes on wire (480 bits), 60 bytes captured (480 bits) on interface 0
IEEE 802.3 Ethernet 
    Destination: CDP/VTP/DTP/PAgP/UDLD (01:00:0c:cc:cc:cc)
    Source: CiscoInc_27:d1:02 (68:bd:ab:27:d1:02)
    Length: 34
    Padding: 000000000000000000000000
Logical-Link Control
Dynamic Trunk Protocol:  (Operating/Administrative): Trunk/On (0x81) (Operating/Administrative): 802.1Q/802.1Q (0xa5): 68:bd:ab:27:d1:02
    Version: 1
    Domain
        Type: Domain (0x0001)
        Length: 5
        Domain: 
    Trunk Status
        Type: Trunk Status (0x0002)
        Length: 5
        Value: Trunk/On (0x81)
            1... .... = Trunk Operating Status: Trunk (0x01)
            .... .001 = Trunk Administrative Status: On (0x01)
    Trunk Type
        Type: Trunk Type (0x0003)
        Length: 5
        Value: 802.1Q/802.1Q (0xa5)
            101. .... = Trunk Operating Type: 802.1Q (0x05)
            .... .101 = Trunk Administrative Type: 802.1Q (0x05)
    Sender ID
        Type: Sender ID (0x0004)
        Length: 10
        Sender ID: CiscoInc_27:d1:02 (68:bd:ab:27:d1:02)


## Tests

### dynamic auto <> dynamic auto
> SW1: Administrative Mode: dynamic auto
> SW1: Operational Mode: static access
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: dynamic auto
> SW2: Operational Mode: static access
> SW2: Negotiation of Trunking: On

DTP Packet on wire but no trunk will be negotiated = *** Access Port***


### dynamic desirable <> dynamic auto
> SW1: Administrative Mode: dynamic desirable
> SW1: Operational Mode: trunk
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: dynamic auto
> SW2: Operational Mode: trunk
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: dot1q
> SW2: Negotiation of Trunking: On

*** trunk ***

### dynamic desirable <> dynamic desirable
> SW1: Administrative Mode: dynamic desirable
> SW1: Operational Mode: trunk
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: dynamic desirable
> SW2: Operational Mode: trunk
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: dot1q
> SW2: Negotiation of Trunking: On

*** trunk ***

### trunk <> dynamic auto
> SW1: Administrative Mode: trunk
> SW1: Operational Mode: trunk
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: dynamic auto
> SW2: Operational Mode: trunk
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: dot1q
> SW2: Negotiation of Trunking: On

*** trunk***


## trunk <> dynamic desirable
> SW1: Administrative Mode: trunk
> SW1: Operational Mode: trunk
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: dynamic desirable
> SW2: Operational Mode: trunk
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: dot1q
> SW2: Negotiation of Trunking: On

***trunk***

## trunk <> trunk
> SW1: Administrative Mode: trunk
> SW1: Operational Mode: trunk
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: trunk
> SW2: Operational Mode: trunk
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: dot1q
> SW2: Negotiation of Trunking: On

***trunk***


## trunk <> access
> SW1: Administrative Mode: trunk
> SW1: Operational Mode: trunk
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: static access
> SW2: Operational Mode: static access
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: native
> SW2: Negotiation of Trunking: Off

*Mar  1 00:42:18.040: %LINK-3-UPDOWN: Interface GigabitEthernet0/2, changed state to up
*Mar  1 00:42:18.040: %SPANTREE-7-RECV_1Q_NON_TRUNK: Received 802.1Q BPDU on non trunk GigabitEthernet0/2 VLAN1.
*Mar  1 00:42:18.040: %SPANTREE-7-BLOCK_PORT_TYPE: Blocking GigabitEthernet0/2 on VLAN0001. Inconsistent port type.
*Mar  1 00:42:19.047: %LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/2, changed state to up
> Spanning Tree blocks the access port (TYPE_Inc)

> without cdp both ports are up in spanning tree

***trunk / access***

### dynamic desirable (VTP domain "lab1") <> dynamic auto (VTP domain "lab2")
> SW1: Administrative Mode: dynamic desirable
> SW1: Operational Mode: static access
> SW1: Administrative Trunking Encapsulation: dot1q
> SW1: Operational Trunking Encapsulation: dot1q
> SW1: Negotiation of Trunking: On

> SW2: Administrative Mode: dynamic auto
> SW2: Operational Mode: static access
> SW2: Administrative Trunking Encapsulation: dot1q
> SW2: Operational Trunking Encapsulation: dot1q
> SW2: Negotiation of Trunking: On

***access***


## Comands

`switchport nonegotiate` only acceptalbe on access or trunk ports 


## Verification

```
Switch#show interfaces gigabitEthernet 0/7 switchport
Name: Gi0/7
Switchport: Enabled
Administrative Mode: dynamic auto
Operational Mode: trunk
Administrative Trunking Encapsulation: dot1q
Operational Trunking Encapsulation: dot1q
Negotiation of Trunking: On
Access Mode VLAN: 1 (default)
Trunking Native Mode VLAN: 1 (default)
Administrative Native VLAN tagging: enabled
Voice VLAN: none
Administrative private-vlan host-association: none
Administrative private-vlan mapping: none
Administrative private-vlan trunk native VLAN: none
Administrative private-vlan trunk Native VLAN tagging: enabled
Administrative private-vlan trunk encapsulation: dot1q
Administrative private-vlan trunk normal VLANs: none
Administrative private-vlan trunk associations: none
Administrative private-vlan trunk mappings: none
Operational private-vlan: none
Trunking VLANs Enabled: ALL
Pruning VLANs Enabled: 2-1001
Capture Mode Disabled
Capture VLANs Allowed: ALL

Protected: false
Unknown unicast blocked: disabled
Unknown multicast blocked: disabled
Appliance trust: none
```