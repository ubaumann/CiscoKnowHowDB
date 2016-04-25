+ access-group
  + Specify access control for packets
  + <1-199>
    + IP access list (standard or extended)
    + in
      + inbound packets
        + <cr>
  + <1300-2699>
    + IP expanded access list (standard or extended)
    + in
      + inbound packets
        + <cr>
  + WORD
    + Access-list name
    + in
      + inbound packets
        + <cr>
+ admission
  + Apply Network Admission Control
  + WORD
    + Name of authenticaion/admission rule
      + <cr>
+ arp
  + Configure ARP features
  + inspection
    + Arp Inspection configuration
    + limit
      + Configure Rate limit of incoming ARP packets
      + none
        + No limit
          + <cr>
      + rate
        + Rate Limit
        + <0-2048>
          + Packets per second
          + burst
            + Configure Burst parameters for ARP packets
            + interval
              + Number of seconds to check the rate
              + <1-15>
                + Burst interval in seconds
                  + <cr>
            + <cr>
    + trust
      + Configure Trust state
        + <cr>
+ auth-proxy
  + Apply authenticaton proxy
  + WORD
    + Name of authenticaion/admission rule
      + <cr>
+ device
  + IP device tracking
  + tracking
    + IP device tracking
    + maximum
      + IP device tracking maximum
      + <1-10>
        + Maximum devices
          + <cr>
+ dhcp
  + Configure DHCP parameters for this interface
  + client
    + DHCP client configuration
    + class-id
      + Specify Class-ID to use
      + WORD
        + Class-ID string
          + <cr>
      + hex
        + Specify hexadecimal class-ID
        + Hex-string
          + Class-ID in hex
    + client-id
      + Specify Client-ID to use
      + Async
        + Async interface
        + <1-0>
          + Async interface number
      + Auto-Template
        + Auto-Template interface
        + <1-999>
          + Auto-Template interface number
      + BVI
        + Bridge-Group Virtual Interface
        + <1-255>
          + BVI interface number
      + CTunnel
        + CTunnel interface
        + <0-2147483647>
          + CTunnel interface number
      + Dialer
        + Dialer interface
        + <0-255>
          + Dialer interface number
      + FastEthernet
        + FastEthernet IEEE 802.3
        + <0-0>
          + FastEthernet interface number
            + <cr>
      + Filter
        + Filter interface
        + <0-0>
          + Filter interface number
      + Filtergroup
        + Filter Group interface
        + <0-0>
          + Filtergroup interface number
      + GigabitEthernet
        + GigabitEthernet IEEE 802.3z
        + <0-0>
          + GigabitEthernet interface number
            + <cr>
      + GroupVI
        + Group Virtual interface
        + <1-255>
          + GroupVI interface number
      + Lex
        + Lex interface
        + <0-2147483647>
          + Lex interface number
      + Loopback
        + Loopback interface
        + <0-2147483647>
          + Loopback interface number
            + <cr>
      + Null
        + Null interface
        + <0-0>
          + Null interface number
      + Port-channel
        + Ethernet Channel of interfaces
        + <1-48>
          + Port-channel interface number
            + <cr>
      + Portgroup
        + Portgroup interface
        + <0-0>
          + Portgroup interface number
      + Pos-channel
        + POS Channel of interfaces
        + <1-4094>
          + Pos-channel interface number
      + Tunnel
        + Tunnel interface
        + <0-2147483647>
          + Tunnel interface number
            + <cr>
      + Vif
        + PGM Multicast Host interface
        + <1-1>
          + Vif interface number
      + Virtual-Template
        + Virtual Template interface
        + <1-200>
          + Virtual-Template interface number
      + Virtual-TokenRing
        + Virtual TokenRing
        + <0-2147483647>
          + Virtual-TokenRing interface number
      + Vlan
        + Catalyst Vlans
        + <1-4094>
          + Vlan interface number
            + <cr>
      + ascii
        + Client-ID as ascii string
        + WORD
          + Client-ID string
            + <cr>
      + fcpa
        + Fiber Channel
        + <0-0>
          + fcpa interface number
      + hex
        + Client-ID in hex
        + Hex-string
          + Client-ID in hex
    + hostname
      + Specify hostname to use
      + WORD
        + Hostname string
          + <cr>
    + lease
      + Requested address lease time
      + <0-365>
        + Days
        + <0-23>
          + Hours
          + <0-59>
            + Minutes
              + <cr>
            + <cr>
          + <cr>
    + request
      + Specify options (not) to request
      + dns-nameserver
        + DNS nameserver (6)
        + domain-name
          + Domain name (15)
          + netbios-nameserver
            + NETBIOS nameserver (44)
            + router
              + Default router option (3)
              + static-route
                + Static route option (33)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + router
                + Default router option (3)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + router
            + Default router option (3)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + static-route
                + Static route option (33)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + static-route
            + Static route option (33)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + router
                + Default router option (3)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + tftp-server-address
            + TFTP server address (150)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + vendor-specific
            + Vendor specific option (43)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
            + <cr>
        + netbios-nameserver
          + NETBIOS nameserver (44)
          + domain-name
            + Domain name (15)
            + router
              + Default router option (3)
              + static-route
                + Static route option (33)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + router
                + Default router option (3)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + router
            + Default router option (3)
            + domain-name
              + Domain name (15)
              + static-route
                + Static route option (33)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + static-route
            + Static route option (33)
            + domain-name
              + Domain name (15)
              + router
                + Default router option (3)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + tftp-server-address
            + TFTP server address (150)
            + domain-name
              + Domain name (15)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + vendor-specific
            + Vendor specific option (43)
            + domain-name
              + Domain name (15)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
            + <cr>
        + router
          + Default router option (3)
          + domain-name
            + Domain name (15)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + static-route
                + Static route option (33)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + netbios-nameserver
            + NETBIOS nameserver (44)
            + domain-name
              + Domain name (15)
              + static-route
                + Static route option (33)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + static-route
            + Static route option (33)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + tftp-server-address
            + TFTP server address (150)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + vendor-specific
            + Vendor specific option (43)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
            + <cr>
        + static-route
          + Static route option (33)
          + domain-name
            + Domain name (15)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + router
                + Default router option (3)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + netbios-nameserver
            + NETBIOS nameserver (44)
            + domain-name
              + Domain name (15)
              + router
                + Default router option (3)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + router
            + Default router option (3)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + tftp-server-address
                  + TFTP server address (150)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + tftp-server-address
            + TFTP server address (150)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + vendor-specific
            + Vendor specific option (43)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + tftp-server-address
                    + TFTP server address (150)
                      + <cr>
                    + <cr>
                + tftp-server-address
                  + TFTP server address (150)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + tftp-server-address
                + TFTP server address (150)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + tftp-server-address
              + TFTP server address (150)
              + domain-name
                + Domain name (15)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
            + <cr>
        + tftp-server-address
          + TFTP server address (150)
          + domain-name
            + Domain name (15)
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + netbios-nameserver
            + NETBIOS nameserver (44)
            + domain-name
              + Domain name (15)
              + router
                + Default router option (3)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + router
              + Default router option (3)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + static-route
              + Static route option (33)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + vendor-specific
              + Vendor specific option (43)
              + domain-name
                + Domain name (15)
                + router
                  + Default router option (3)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                  + <cr>
              + router
                + Default router option (3)
                + domain-name
                  + Domain name (15)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + domain-name
                  + Domain name (15)
                  + router
                    + Default router option (3)
                      + <cr>
                    + <cr>
                + router
                  + Default router option (3)
                  + domain-name
                    + Domain name (15)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
              + <cr>
          + router
            + Default router option (3)
            + domain-name
              + Domain name (15)
              + netbios-nameserver
                + NETBIOS nameserver (44)
                + static-route
                  + Static route option (33)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                  + <cr>
              + static-route
                + Static route option (33)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + vendor-specific
                    + Vendor specific option (43)
                      + <cr>
                    + <cr>
                + vendor-specific
                  + Vendor specific option (43)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
              + vendor-specific
                + Vendor specific option (43)
                + netbios-nameserver
                  + NETBIOS nameserver (44)
                  + static-route
                    + Static route option (33)
                      + <cr>
                    + <cr>
                + static-route
                  + Static route option (33)
                  + netbios-nameserver
                    + NETBIOS nameserver (44)
                      + <cr>
                    + <cr>
                  + <cr>
                + <cr>
            + netbios-nameserver
              + NETBIOS nameserver (44)
              + domain-name
                + Domain name (15)
                + static-route
                  + Static route option (33)