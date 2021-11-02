# Networking Overview

A networking enables two computers to communicate with each other.

There is wide array of :

1. Topologies
    - Mesh
    - Tree
    - Star
2. Mediums
    - Ethernet
    - Fiber
    - Coax
    - Wireless
3. Protocols
    - TCP
    - UDP
    - IPX

Setting up large, flat network is not extremely difficult and it can be a reliable network at least operationally.

 

Flat network is like building a house on a land plot and considering it secure because it has a lock on the door. 

By creating lots of smaller networks and having them communicate, we can add defense layers. 

Pivoting around a network is not difficult, but doing it quickly and silently is tough and will slow attackers down. 

## Example → 1

Building smaller networks and putting Access Control lists around them is like putting fence around the property's border that creates an specific entry and exit points.

Yes, an attacker can jump over fence but this look suspicious and is not common, allowing it to be quickly detected as malicious activity.

**Question → Why is the printer network talking to the server over HTTP ?** 

 

## Example → 2

Take time to document each network's purpose is like placing lights around the property, making sure all activities can be seen. 

**Question → Why is the printer network talking to the internet at all ?**

## Example → 3

Intrusion Detection System like Suricata or Snort are deterrent to running network scans.     **Deterrent → defensive**