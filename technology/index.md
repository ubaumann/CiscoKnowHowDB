# CCIE Blue Print Routing and Switching Lab Exam Version 5.0

## 1.0 Layer 2 Technologies

###1.1 LAN switching technologies
    
1. Implement and troubleshoot switch administration                    
  1.Managing MAC address table
  2. errdisable recovery
  3. L2 MTU
2. Implement and troubleshoot layer 2 protocols                    
  1. CDP, LLDP
  2. UDLD
3. Implement and troubleshoot VLAN                    
  1. access ports
  2. VLAN database
  3. normal, extended VLAN, voice VLAN
4. Implement and troubleshoot trunking                    
  1. VTPv1, VTPv2, VTPv3, VTP pruning
  2. dot1Q
  3. Native VLAN
  4. Manual pruning
5. Implement and troubleshoot etherchannel                    
  1. LACP, PAgP, manual
  2. layer 2, layer 3
  3. load-balancing
  4. etherchannel misconfiguration guard
6. Implement and troubleshoot spanning-tree                    
  1. PVST+/RPVST+/MST
  2. switch priority, port priority, path cost, STP timers
  3. port fast, BPDUguard, BPDUfilter
  4. loopguard, rootguard
7. Implement and troubleshoot other LAN switching technologies                    
  1. SPAN, RSPAN, ERSPAN

### 1.2 Layer 2 Multicast
    
1. Implement and troubleshoot IGMP                         
  1. IGMPv1, IGMPv2, IGMPv3
  2. IGMP snooping
  3. IGMP querier
  4. IGMP filter
  5. IGMP proxy

### 1.3 Layer 2 WAN circuit technologies
    
1. Implement and troubleshoot HDLC
2. Implement and troubleshoot PPP                  
  1. authentication [PAP, CHAP]
  2. PPPoE
  3. MLPPP

### 1.4 Troubleshooting layer 2 technologies
    
1. Use IOS troubleshooting tools                    
  1. debug, conditional debug
  2. ping, traceroute with extended options
  3. Embedded packet capture
2. Apply troubleshooting methodologies                    
  1. Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
  2. Design and implement valid solutions according to constraints
  3. Verify and monitor resolution
3. Interpret packet capture                    
  1. Using wireshark trace analyzer
  2. Using IOS embedded packet capture

## 2.0 Layer 3 Technologies

### 2.1 Addressing technologies
    
1. Identify, implement and troubleshoot IPv4 addressing and sub-netting                    
  1. Address types, VLSM
  2. ARP
2. Identify, implement and troubleshoot IPv6 addressing and sub-netting                  
  1. Unicast, multicast
  2. EUI-64
  3. ND, RS/RA
  4. Autoconfig/SLAAC temporary addresses [RFC4941]
  5. Global prefix configuration feature

### 2.2 Layer 3 Multicast
    
1. Troubleshoot reverse path forwarding                    
  1. RPF failure
  2. RPF failure with tunnel interface
2. Implement and troubleshoot IPv4 protocol independent multicast                    
  1. PIM dense mode, sparse mode, sparse-dense mode
  2. Static RP, auto-RP, BSR
  3. Bidirectional PIM
  4. Source-specific multicast
  5. Group to RP mapping
  6. Multicast boundary
3. Implement and troubleshoot multicast source discovery protocol                  
  1. Intra-domain MSDP [anycast RP]
  2. SA filter

### 2.3 Fundamental routing concepts
    
1. Implement and troubleshoot static routing
2. Implement and troubleshoot default routing
3. Compare routing protocol types                    
  1. distance vector
  2. link state
  3. path vector
4. Implement, optimize and troubleshoot administrative distance
5. Implement and troubleshoot passive interface
6. Implement and troubleshoot VRF lite
7. Implement, optimize and troubleshoot filtering with any routing protocol
8. Implement, optimize and troubleshoot redistribution between any routing protocol
9. Implement, optimize and troubleshoot manual and auto summarization with any routing protocol
10. Implement, optimize and troubleshoot policy-based routing
11. Identify and troubleshoot sub-optimal routing
12. Implement and troubleshoot bidirectional forwarding detection
13. Implement and troubleshoot loop prevention mechanisms                    
  1. Route tagging, filtering
  2. Split horizon
  3. Route poisoning
14. Implement and troubleshoot routing protocol authentication                         
  1. MD5
  2. key-chain
  3. EIGRP HMAC SHA2-256bit
  4. OSPFv2 SHA1-196bit
  5. OSPFv3 IPsec authentication

### 2.4 RIP v2
    
1. Implement and troubleshoot RIPv2

### 2.5 EIGRP [for IPv4 and IPv6]
    
1. Describe packet types                    
  1. Packet types [hello, query, update, and such]
  2. Route types [internal, external]
2. Implement and troubleshoot neighbor relationship                    
  1. Multicast, unicast EIGRP peering
3. Implement and Troubleshoot Loop free path selection                    
  1. RD, FD, FC, successor, feasible successor
  2. Classic metric
  3. Wide metric
4. Implement and troubleshoot operations                    
  1. General operations
  2. Topology table, update, query, active, passive
  3. Stuck in active
  4. Graceful shutdown
5. Implement and troubleshoot EIGRP stub                    
  1. stub
  2. leak-map
6. Implement and troubleshoot load-balancing                    
  1. equal-cost
  2. unequal-cost
  3. add-path
7. Implement EIGRP [multi-address] named mode                    
  1. Types of families
  2. IPv4 address-family
  3. IPv6 address-family
8. Implement, troubleshoot and optimize EIGRP convergence and scalability                  
  1. Describe fast convergence requirements
  2. Control query boundaries
  3. IP FRR/fast reroute [single hop]
  4. Summary leak-map
  5. Summary metric

### 2.6 OSPF [v2 and v3]
    
1. Describe packet types                    
  1. LSA types [1, 2, 3, 4, 5, 7, 9]
  2. Route types [N1, N2, E1, E2]
2. Implement and troubleshoot neighbor relationship
3. Implement and troubleshoot OSPFv3 address-family support                    
  1. IPv4 address-family
  2. IPv6 address-family
4. Implement and troubleshoot network types, area types and router types                    
  1. Point-to-point, multipoint, broadcast, non-broadcast
  2. LSA types, area type: backbone, normal, transit, stub, NSSA, totally stub
  3. Internal router, ABR, ASBR
  4. Virtual link
5. Implement and troubleshoot path preference
6. Implement and troubleshoot operations                    
  1. General operations
  2. Graceful shutdown
  3. GTSM [generic TTL security mechanism]
7. Implement, troubleshoot and optimize OSPF convergence and scalability                  
  1. Metrics
  2. LSA throttling, SPF tuning, fast hello
  3. LSA propagation control [area types, ISPF]
  4. IP FR/fast reroute [single hop]
  5. LFA/loop-free alternative [multi hop]
  6. OSPFv3 prefix suppression

### 2.7 BGP
    
1. Describe, implement and troubleshoot peer relationships                    
  1. Peer-group, template
  2. Active, passive
  3. States, timers
  4. Dynamic neighbors
2. Implement and troubleshoot IBGP and EBGP                    
  1. EBGP, IBGP
  2. 4 bytes AS number
  3. Private AS
3. Explain attributes and best-path selection
4. Implement, optimize and troubleshoot routing policies                    
  1. Attribute manipulation
  2. Conditional advertisement
  3. Outbound route filtering
  4. Communities, extended communities
  5. Multi-homing
5. Implement and troubleshoot scalability                    
  1. Route-reflector, cluster
  2. Confederations
  3. Aggregation, AS set
6. Implement and troubleshoot multi-protocol BGP                    
  1. IPv4, IPv6, VPN address-family
7. Implement and troubleshoot AS path manipulations                    
  1. Local AS, allow AS in, remove private AS
  2. Prepend
  3. Regexp
8. Implement and Troubleshoot Other Features                  
  1. Multipath
  2. BGP synchronization
  3. Soft reconfiguration, route refresh

### 2.8 Troubleshooting layer 3 technologies
    
1. Use IOS troubleshooting tools                    
  1. debug, conditional debug
  2. ping, traceroute with extended options
  3. Embedded packet capture
2. Apply troubleshooting methodologies                    
  1. Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
  2. Design and implement valid solutions according to constraints
  3. Verify and monitor resolution
3. Interpret packet capture                    
  1. Using wireshark trace analyzer
  2. Using IOS embedded packet capture

## 3.0 VPN Technologies

### 3.1 Tunneling
    
1. Implement and troubleshoot MPLS operations                    
  1. Label stack, LSR, LSP
  2. LDP
  3. MPLS ping, MPLS traceroute
2. Implement and troubleshoot basic MPLS L3VPN                    
  1. L3VPN, CE, PE, P
  2. Extranet [route leaking]
3. Implement and troubleshoot encapsulation                    
  1. GRE
  2. Dynamic GRE
4. Implement and troubleshoot DMVPN [single hub]                    
  1. NHRP
  2. DMVPN with IPsec using preshared key
  3. QoS profile
  4. Pre-classify

### 3.2 Encryption
    
1. Implement and troubleshoot IPsec with preshared key                             
  1. IPv4 site to IPv4 site
  2. IPv6 in IPv4 tunnels
  3. Virtual tunneling interface [VTI]

### 3.3 Troubleshooting VPN technologies
    
1. Use IOS troubleshooting tools                    
  1. debug, conditional debug
  2. ping, traceroute with extended options
  3. Embedded packet capture
2. Apply troubleshooting methodologies                    
  1. Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
  2. Design and implement valid solutions according to constraints
  3. Verify and monitor resolution
3. Interpret packet capture                    
  1. Using wireshark trace analyzer
  2. Using IOS embedded packet capture

## 4.0 Infrastructure Security

### 4.1 Device security
    
1. Implement and troubleshoot IOS AAA using local database
2. Implement and troubleshoot device access control                    
  1. Lines [VTY, AUX, console]
  2. SNMP
  3. Management plane protection
  4. Password encryption
3. Implement and troubleshoot control plane policing

## 4.2 Network security
    
1. Implement and troubleshoot switch security features                    
  1. VACL, PACL
  2. Stormcontrol
  3. DHCP snooping
  4. IP source-guard
  5. Dynamic ARP inspection
  6. Port-security
  7. Private VLAN
2. Implement and troubleshoot router security features                    
  1. IPv4 access control lists [standard, extended, time-based]
  2. IPv6 traffic filter
  3. Unicast reverse path forwarding
3. Implement and troubleshoot IPv6 first hop security                         
  1. RA guard
  2. DHCP guard
  3. Binding table
  4. Device tracking
  5. ND inspection/snooping
  6. Source guard
  7. PACL

## 4.3 Troubleshooting infrastructure security
    
1. Use IOS troubleshooting tools                    
  1. debug, conditional debug
  2. ping, traceroute with extended options
  3. Embedded packet capture
2. Apply troubleshooting methodologies
  1. Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
  2. Design and implement valid solutions according to constraints
  3. Verify and monitor resolution
3. Interpret packet capture                    
  1. Using wireshark trace analyzer
  2. Using IOS embedded packet capture

## 5.0 Infrastructure Services

### 5.1 System management
    
1. Implement and troubleshoot device management                    
  1. Console and VTY
  2. telnet, HTTP, HTTPS, SSH, SCP
  3. [T]FTP
2. Implement and troubleshoot SNMP                    
  1. v2c, v3
3. Implement and troubleshoot logging                           
  1. Local logging, syslog, debug, conditional debug
  2. Timestamp

### 5.2 Quality of service
    
1. Implement and troubleshoot end to end QoS                    
  1. CoS and DSCP mapping
2. Implement, optimize and troubleshoot QoS using MQC                         
  1. Classification
  2. Network based application recognition [NBAR]
  3. Marking using IP precedence, DSCP, CoS, ECN
  4. Policing, shaping
  5. Congestion management [queuing]
  6. HQoS, sub-rate ethernet link
  7. Congestion avoidance [WRED]

### 5.3 Network services
    
1. Implement and troubleshoot first-hop redundancy protocols                    
  1. HSRP, GLBP, VRRP
  2. Redundancy using IPv6 RS/RA
2. Implement and troubleshoot network time protocol                    
  1. NTP master, client, version 3, version 4
  2. NTP authentication
3. Implement and troubleshoot IPv4 and IPv6 DHCP                    
  1. DHCP client, IOS DHCP server, DHCP relay
  2. DHCP options
  3. DHCP protocol operations
  4. SLAAC/DHCPv6 interaction
  5. Stateful, stateless DHCPv6
  6. DHCPv6 prefix delegation
4. Implement and troubleshoot IPv4 network address translation                  
  1. Static NAT, dynamic NAT, policy-based NAT, PAT
  2. NAT ALG

### 5.4 Network optimization
    
1. Implement and troubleshoot IP SLA                    
  1. ICMP, UDP, jitter, VoIP
2. Implement and troubleshoot tracking object                    
  1. Tracking object, tracking list
  2. Tracking different entities [e.g. interfaces, routes, IPSLA, and such]
3. Implement and troubleshoot netflow                  
  1. Netflow v5, v9
  2. Local retrieval
  3. Export [configuration only]
4. Implement and troubleshoot embedded event manager
  1. EEM policy using applet

### 5.5 Troubleshooting infrastructure services
    
1. Use IOS troubleshooting tools                    
  1. debug, conditional debug
  2. ping, traceroute with extended options
  3. Embedded packet capture
2. Apply troubleshooting methodologies                    
  1. Diagnose the root cause of networking issue [analyze symptoms, identify and describe root cause]
  2. Design and implement valid solutions according to constraints
  3. Verify and monitor resolution
3. Interpret packet capture          
  1. Using wireshark trace analyzer
  2. Using IOS embedded packet capture
