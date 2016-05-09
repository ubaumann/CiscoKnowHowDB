# Spanning-Tree

## ToDo


## Features

### bpdu filter
Port doesn't send out bpdu's

- Global configuration 
  - `spanning-tree portfast bpdufilter default`
    - If a BPDU is received on a Port Fast-enabled interface, the interface loses its Port Fast-operational status, and BPDU filtering is disabled.

- Port configuration
  - `spanning-tree bpdufilter enable`
  - `spanning-tree bpdufilter disabled`
  - `no` | `default spanning-tree bpdufiler`  
  
> Enabling BPDU filtering on an interface is the same as disabling spanning tree on it and can result in
spanning-tree loops.

### verification

```
s1#show spanning-tree interface fa 0/5 detail
 Port 5 (FastEthernet0/5) of VLAN0001 is designated forwarding
   Port path cost 19, Port priority 128, Port Identifier 128.5.
   Designated root has priority 24577, address f025.72d1.b880
   Designated bridge has priority 24577, address f025.72d1.b880
   Designated port id is 128.5, designated path cost 0
   Timers: message age 0, forward delay 0, hold 0
   Number of transitions to forwarding state: 1
   Link type is point-to-point by default
   Bpdu filter is enabled
   BPDU: sent 6305, received 0
```

