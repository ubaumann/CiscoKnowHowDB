# CCIE Blue Print Routing and Switching Lab Exam Version 5.0

## 1.0 Layer 2 Technologies

###1.1 LAN switching technologies
    
1.1.a Implement and troubleshoot switch administration                    
1.1.a [i] Managing MAC address table
1.1.a [ii] errdisable recovery
1.1.a [iii] L2 MTU
1.1.b Implement and troubleshoot layer 2 protocols                    
1.1.b [i] CDP, LLDP
1.1.b [ii] UDLD
1.1.c Implement and troubleshoot VLAN                    
1.1.c [i] access ports
1.1.c [ii] VLAN database
1.1.c [iii] normal, extended VLAN, voice VLAN
1.1.d Implement and troubleshoot trunking                    
1.1.d [i] VTPv1, VTPv2, VTPv3, VTP pruning
1.1.d [ii] dot1Q
1.1.d [iii] Native VLAN
1.1.d [iv] Manual pruning
1.1.e Implement and troubleshoot etherchannel                    
1.1.e [i] LACP, PAgP, manual
1.1.e [ii] layer 2, layer 3
1.1.e [iii] load-balancing
1.1.e [iv] etherchannel misconfiguration guard
1.1.f Implement and troubleshoot spanning-tree                    
1.1.f [i] PVST+/RPVST+/MST
1.1.f [ii] switch priority, port priority, path cost, STP timers
1.1.f [iii] port fast, BPDUguard, BPDUfilter
1.1.f [iv] loopguard, rootguard
1.1.g Implement and troubleshoot other LAN switching technologies                    
1.1.g [i] SPAN, RSPAN, ERSPAN

### 1.2 Layer 2 Multicast
    
1.2.a Implement and troubleshoot IGMP                         
1.2.a [I] IGMPv1, IGMPv2, IGMPv3
1.2.a [ii] IGMP snooping
1.2.a [iii] IGMP querier
1.2.a [iv] IGMP filter
1.2.a [v] IGMP proxy

### 1.3 Layer 2 WAN circuit technologies
    
1.3.a Implement and troubleshoot HDLC
1.3.b Implement and troubleshoot PPP                  
1.3.b [i] authentication [PAP, CHAP]
1.3.b [ii] PPPoE
1.3.b [iii] MLPPP
### 1.4 Troubleshooting layer 2 technologies
    
1.4.a Use IOS troubleshooting tools                    
1.4.a [i] debug, conditional debug
1.4.a [ii] ping, traceroute with extended options
1.4.a [iii] Embedded packet capture
1.4.b Apply troubleshooting methodologies                    
1.4.b [i] Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
1.4.b [ii] Design and implement valid solutions according to constraints
1.4.b [iii] Verify and monitor resolution
1.4.c Interpret packet capture                    
1.4.c [i] Using wireshark trace analyzer
1.4.c [ii] Using IOS embedded packet capture


## 2.0 Layer 3 Technologies

### 2.1 Addressing technologies
    
2.1.a Identify, implement and troubleshoot IPv4 addressing and sub-netting                    
2.1.a [i] Address types, VLSM
2.1.a [ii] ARP
2.1.b Identify, implement and troubleshoot IPv6 addressing and sub-netting                  
2.1.b [i] Unicast, multicast
2.1.b [ii] EUI-64
2.1.b [iii] ND, RS/RA
2.1.b [iv] Autoconfig/SLAAC temporary addresses [RFC4941]
2.1.b [v] Global prefix configuration feature
2.2 Layer 3 Multicast
    
2.2.a Troubleshoot reverse path forwarding                    
2.2.a [i] RPF failure
2.2.a[ii] RPF failure with tunnel interface
2.2.b Implement and troubleshoot IPv4 protocol independent multicast                    
2.2.b [i] PIM dense mode, sparse mode, sparse-dense mode
2.2.b [ii] Static RP, auto-RP, BSR
2.2.b [iii] Bidirectional PIM
2.2.b [iv] Source-specific multicast
2.2.b [v] Group to RP mapping
2.2.b [vi] Multicast boundary
2.2.c Implement and troubleshoot multicast source discovery protocol                  
2.2.c.[i] Intra-domain MSDP [anycast RP]
2.2.c.[ii] SA filter

### 2.3 Fundamental routing concepts
    
2.3.a Implement and troubleshoot static routing
2.3.b Implement and troubleshoot default routing
2.3.c Compare routing protocol types                    
2.3.c [i] distance vector
2.3.c [ii] link state
2.3.c [iii] path vector
2.3.d Implement, optimize and troubleshoot administrative distance
2.3.e Implement and troubleshoot passive interface
2.3.f Implement and troubleshoot VRF lite
2.3.g Implement, optimize and troubleshoot filtering with any routing protocol
2.3.h Implement, optimize and troubleshoot redistribution between any routing protocol
2.3.i Implement, optimize and troubleshoot manual and auto summarization with any routing protocol
2.3.j Implement, optimize and troubleshoot policy-based routing
2.3.k Identify and troubleshoot sub-optimal routing
2.3.l Implement and troubleshoot bidirectional forwarding detection
2.3.m Implement and troubleshoot loop prevention mechanisms                    
2.3.m [i] Route tagging, filtering
2.3.m [ii] Split horizon
2.3.m [iii] Route poisoning
2.3.n Implement and troubleshoot routing protocol authentication                         
2.3.n [i] MD5
2.3.n [ii] key-chain
2.3.n [iii] EIGRP HMAC SHA2-256bit
2.3.n [iv] OSPFv2 SHA1-196bit
2.3.n [v] OSPFv3 IPsec authentication

### 2.4 RIP v2
    
2.4.a Implement and troubleshoot RIPv2

### 2.5 EIGRP [for IPv4 and IPv6]
    
2.5.a Describe packet types                    
2.5.a [i] Packet types [hello, query, update, and such]
2.5.a [ii] Route types [internal, external]
2.5.b Implement and troubleshoot neighbor relationship                    
2.5.b [i] Multicast, unicast EIGRP peering
2.5.c Implement and Troubleshoot Loop free path selection                    
2.5.c [i] RD, FD, FC, successor, feasible successor
2.5.c [ii] Classic metric
2.5.c [iii] Wide metric
2.5.d Implement and troubleshoot operations                    
2.5.d [i] General operations
2.5.d [ii] Topology table, update, query, active, passive
2.5.d [iii] Stuck in active
2.5.d [iv] Graceful shutdown
2.5.e Implement and troubleshoot EIGRP stub                    
2.5.e [i] stub
2.5.e [ii] leak-map
2.5.f Implement and troubleshoot load-balancing                    
2.5.f [i] equal-cost
2.5.f [ii] unequal-cost
2.5.f [iii] add-path
2.5.g Implement EIGRP [multi-address] named mode                    
2.5.g [i] Types of families
2.5.g [ii] IPv4 address-family
2.5.g [iii] IPv6 address-family
2.5.h Implement, troubleshoot and optimize EIGRP convergence and scalability                  
2.5.h [i] Describe fast convergence requirements
2.5.h [ii] Control query boundaries
2.5.h [iii] IP FRR/fast reroute [single hop]
2.5.h [iv] Summary leak-map
2.5.h [v] Summary metric

### 2.6 OSPF [v2 and v3]
    
2.6.a Describe packet types                    
2.6.a [i] LSA types [1, 2, 3, 4, 5, 7, 9]
2.6.a [ii] Route types [N1, N2, E1, E2]
2.6.b Implement and troubleshoot neighbor relationship
2.6.c Implement and troubleshoot OSPFv3 address-family support                    
2.6.c [i] IPv4 address-family
2.6.c [ii] IPv6 address-family
2.6.d Implement and troubleshoot network types, area types and router types                    
2.6.d [i] Point-to-point, multipoint, broadcast, non-broadcast
2.6.d [ii] LSA types, area type: backbone, normal, transit, stub, NSSA, totally stub
2.6.d [iii] Internal router, ABR, ASBR
2.6.d [iv] Virtual link
2.6.e Implement and troubleshoot path preference
2.6.f Implement and troubleshoot operations                    
2.6.f [i] General operations
2.6.f [ii] Graceful shutdown
2.6.f [iii] GTSM [generic TTL security mechanism]
2.6.g Implement, troubleshoot and optimize OSPF convergence and scalability                  
2.6.g [i] Metrics
2.6.g [ii] LSA throttling, SPF tuning, fast hello
2.6.g [iii] LSA propagation control [area types, ISPF]
2.6.g [iv] IP FR/fast reroute [single hop]
2.6.g [v] LFA/loop-free alternative [multi hop]
2.6.g [vi] OSPFv3 prefix suppression

### 2.7 BGP
    
2.7.a Describe, implement and troubleshoot peer relationships                    
2.7.a [i] Peer-group, template
2.7.a [ii] Active, passive
2.7.a [iii] States, timers
2.7.a [iv] Dynamic neighbors
2.7.b Implement and troubleshoot IBGP and EBGP                    
2.7.b [i] EBGP, IBGP
2.7.b [ii] 4 bytes AS number
2.7.b [iii] Private AS
2.7.c Explain attributes and best-path selection
2.7.d Implement, optimize and troubleshoot routing policies                    
2.7.d [i] Attribute manipulation
2.7.d [ii] Conditional advertisement
2.7.d [iii] Outbound route filtering
2.7.d [iv] Communities, extended communities
2.7.d [v] Multi-homing
2.7.e Implement and troubleshoot scalability                    
2.7.e [i] Route-reflector, cluster
2.7.e [ii] Confederations
2.7.e [iii] Aggregation, AS set
2.7.f Implement and troubleshoot multi-protocol BGP                    
2.7.f [i] IPv4, IPv6, VPN address-family
2.7.g Implement and troubleshoot AS path manipulations                    
2.7.g [i] Local AS, allow AS in, remove private AS
2.7.g [ii] Prepend
2.7.g [iii] Regexp
2.7.h Implement and Troubleshoot Other Features                  
2.7.h [i] Multipath
2.7.h [ii] BGP synchronization
2.7.h [iii] Soft reconfiguration, route refresh

### 2.8 Troubleshooting layer 3 technologies
    
2.8.a Use IOS troubleshooting tools                    
2.8.a [i] debug, conditional debug
2.8.a [ii] ping, traceroute with extended options
2.8.a [iii] Embedded packet capture
2.8.b Apply troubleshooting methodologies                    
2.8.b [i] Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
2.8.b [ii] Design and implement valid solutions according to constraints
2.8.b [iii] Verify and monitor resolution
2.8.c Interpret packet capture                    
2.8.c [i] Using wireshark trace analyzer
2.8.c [ii] Using IOS embedded packet capture


## 3.0 VPN Technologies

### 3.1 Tunneling
    
3.1.a Implement and troubleshoot MPLS operations                    
3.1.a [i] Label stack, LSR, LSP
3.1.a [ii] LDP
3.1.a [iii] MPLS ping, MPLS traceroute
3.1.b Implement and troubleshoot basic MPLS L3VPN                    
3.1.b [i] L3VPN, CE, PE, P
3.1.b [ii] Extranet [route leaking]
3.1.c Implement and troubleshoot encapsulation                    
3.1.c [i] GRE
3.1.c [ii] Dynamic GRE
3.1.d Implement and troubleshoot DMVPN [single hub]                    
3.1.d [i] NHRP
3.1.d [ii] DMVPN with IPsec using preshared key
3.1.d [iii] QoS profile
3.1.d [iv] Pre-classify

### 3.2 Encryption
    
3.2.a Implement and troubleshoot IPsec with preshared key                             
3.2.a [i] IPv4 site to IPv4 site
3.2.a [ii] IPv6 in IPv4 tunnels
3.2.a [iii] Virtual tunneling interface [VTI]

### 3.3 Troubleshooting VPN technologies
    
3.3.a Use IOS troubleshooting tools                    
3.3.a [i] debug, conditional debug
3.3.a [ii] ping, traceroute with extended options
3.3.a [iii] Embedded packet capture
3.3.b Apply troubleshooting methodologies                    
3.3.b [i] Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
3.3.b [ii] Design and implement valid solutions according to constraints
3.3.b [iii] Verify and monitor resolution
3.3.c Interpret packet capture                    
3.3.c [i] Using wireshark trace analyzer
3.3.c [ii] Using IOS embedded packet capture


## 4.0 Infrastructure Security

### 4.1 Device security
    
4.1.a Implement and troubleshoot IOS AAA using local database
4.1.b Implement and troubleshoot device access control                    
4.1.b [i] Lines [VTY, AUX, console]
4.1.b [ii] SNMP
4.1.b [iii] Management plane protection
4.1.b [iv] Password encryption
4.1.c Implement and troubleshoot control plane policing

## 4.2 Network security
    
4.2.a Implement and troubleshoot switch security features                    
4.2.a [i] VACL, PACL
4.2.a [ii] Stormcontrol
4.2.a [iii] DHCP snooping
4.2.a [iv] IP source-guard
4.2.a [v] Dynamic ARP inspection
4.2.a [vi] Port-security
4.2.a [vii] Private VLAN
4.2.b Implement and troubleshoot router security features                    
4.2.b [i] IPv4 access control lists [standard, extended, time-based]
4.2.b [ii] IPv6 traffic filter
4.2.b [iii] Unicast reverse path forwarding
4.2.c Implement and troubleshoot IPv6 first hop security                         
4.2.c [i] RA guard
4.2.c [ii] DHCP guard
4.2.c [iii] Binding table
4.2.c [iv] Device tracking
4.2.c [v] ND inspection/snooping
4.2.c [vi] Source guard
4.2.c [vii] PACL

## 4.3 Troubleshooting infrastructure security
    
4.3.a Use IOS troubleshooting tools                    
4.3.a [i] debug, conditional debug
4.3.a [ii] ping, traceroute with extended options
4.3.a [iii] Embedded packet capture
4.3.b Apply troubleshooting methodologies
4.3.b [i] Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
4.3.b [ii] Design and implement valid solutions according to constraints
4.3.b [iii] Verify and monitor resolution
4.3.c Interpret packet capture                    
4.3.c [i] Using wireshark trace analyzer
4.3.c [ii] Using IOS embedded packet capture


## 5.0 Infrastructure Services

### 5.1 System management
    
5.1.a Implement and troubleshoot device management                    
5.1.a [i] Console and VTY
5.1.a [ii] telnet, HTTP, HTTPS, SSH, SCP
5.1.a [iii] [T]FTP
5.1.b Implement and troubleshoot SNMP                    
5.1.b [i] v2c, v3
5.1.c Implement and troubleshoot logging                           
5.1.c [i] Local logging, syslog, debug, conditional debug
5.1.c [ii] Timestamp

### 5.2 Quality of service
    
5.2.a Implement and troubleshoot end to end QoS                    
5.2.a [i] CoS and DSCP mapping
5.2.b Implement, optimize and troubleshoot QoS using MQC                         
5.2.b [i] Classification
5.2.b [ii] Network based application recognition [NBAR]
5.2.b [iii] Marking using IP precedence, DSCP, CoS, ECN
5.2.b [iv] Policing, shaping
5.2.b [v] Congestion management [queuing]
5.2.b [vi] HQoS, sub-rate ethernet link
5.2.b [vii] Congestion avoidance [WRED]

### 5.3 Network services
    
5.3.a Implement and troubleshoot first-hop redundancy protocols                    
5.3.a [i] HSRP, GLBP, VRRP
5.3.a [ii] Redundancy using IPv6 RS/RA
5.3.b Implement and troubleshoot network time protocol                    
5.3.b [i] NTP master, client, version 3, version 4
5.3.b [ii] NTP authentication
5.3.c Implement and troubleshoot IPv4 and IPv6 DHCP                    
5.3.c [i] DHCP client, IOS DHCP server, DHCP relay
5.3.c [ii] DHCP options
5.3.c [iii] DHCP protocol operations
5.3.c [iv] SLAAC/DHCPv6 interaction
5.3.c [v] Stateful, stateless DHCPv6
5.3.c [vi] DHCPv6 prefix delegation
5.3.d Implement and troubleshoot IPv4 network address translation                  
5.3.d [i] Static NAT, dynamic NAT, policy-based NAT, PAT
5.3.d [ii] NAT ALG

### 5.4 Network optimization
    
5.4.a Implement and troubleshoot IP SLA                    
5.4.a [i] ICMP, UDP, jitter, VoIP
5.4.b Implement and troubleshoot tracking object                    
5.4.b [i] Tracking object, tracking list
5.4.b [ii] Tracking different entities [e.g. interfaces, routes, IPSLA, and such]
5.4.c Implement and troubleshoot netflow                  
5.4.c [i] Netflow v5, v9
5.4.c [ii] Local retrieval
5.4.c [iii] Export [configuration only]
5.4.d Implement and troubleshoot embedded event manager
5.4.d [i] EEM policy using applet

### 5.5 Troubleshooting infrastructure services
    
5.5.a Use IOS troubleshooting tools                    
5.5.a [i] debug, conditional debug
5.5.a [ii] ping, traceroute with extended options
5.5.a [iii] Embedded packet capture
5.5.b Apply troubleshooting methodologies                    
5.5.b [i] Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
5.5.b [ii] Design and implement valid solutions according to constraints
5.5.b [iii] Verify and monitor resolution
5.5.c Interpret packet capture          
5.5.c [i] Using wireshark trace analyzer
5.5.c [ii] Using IOS embedded packet capture
