# 🧮 Networking

## 🌐 Networking Fundamentals
- What is a Network?
- Network Types: LAN, WAN, MAN, PAN
- Packet Switching vs Circuit Switching

### Network Topologies
- Historical topologies: Token Ring, Bus
- Modern topologies: Star, Mesh, Tree, Hybrid

### Network Models
- OSI Model
- TCP/IP Stack

### Network Performance Metrics
- Latency, Jitter, Bandwidth, Throughput
- MTU, MSS

### Broadcast Domain vs Collision Domain
- Definitions, diagrams, and simulations
- Switch segmentation and VLAN boundaries
- Real-world implications in network design

### Message Types: Unicast, Broadcast, Multicast
- Layer 2:
  - MAC unicast, multicast (`01:00:5E`), broadcast (`FF:FF:FF:FF:FF:FF`)
- Layer 3:
  - IP unicast, broadcast (`255.255.255.255`), multicast (`224.0.0.0/4`)
- IGMP and multicast group management
- ARP and DHCP as broadcast examples
- DNS as unicast example
- Practical packet captures using Wireshark

## 🧱 Networking Devices

### Routers
- Static vs dynamic routing
- Default routes
- CIDR and summarization

### Switches
- Spanning Tree Protocol (STP, RSTP, MSTP)
- MAC learning and port forwarding decisions
- VLAN trunking (802.1Q)
- Switchport security features

### Hubs vs Switches
- Historical role of hubs
- Why switches replaced hubs
- Collision domains in hub networks
- Packet flooding vs MAC-based forwarding
- Demo lab: Sniffing on a hub vs switch

### NICs and Interfaces
- Promiscuous mode
- Duplex mismatch issues
- Auto-negotiation

### Firewalls
- Deep Packet Inspection (DPI)
- Zone-based firewall logic
- Common vendor CLI: Cisco ASA, Palo Alto

### Load Balancers
- Algorithms: Round-robin, least connections
- Health checks
- Application awareness (SSL termination)

### Wireless Infrastructure
- SSIDs, channels, encryption (WEP, WPA2, WPA3)
- 2.4 GHz vs 5 GHz vs 6 GHz bands
- Access Point roles (controller-based, standalone)

### Modems and Gateways
- DSL, Cable, Fiber modems
- NAT behavior in gateways
- Dual NAT and CGNAT explained

## 🏗️ OSI Model Layers 

### Physical Layer
- Cable standards: Cat5e, Cat6, Cat6a, Cat7
- Fiber optic types: single-mode, multi-mode
- Signal degradation and attenuation
- Bit-level transmission simulation

### Data Link Layer
- Ethernet frame breakdown: Preamble, SFD, MACs, Type, FCS
- Switch loop protection (STP, BPDU Guard)
- VLAN tagging and double tagging (Q-in-Q)
- MAC flooding attacks (brief intro)

### Network Layer
- IPv4 fragmentation and reassembly
- Subnetting techniques and exercises
- Route redistribution concepts
- NAT types (static, dynamic, PAT)
- Layer 3 ACLs and firewalling

### Transport Layer
- TCP handshake deep dive (SYN, SYN-ACK, ACK)
- Retransmission and sliding window mechanics
- UDP with practical examples: TFTP, SNMP
- Port scans: SYN, FIN, NULL, Xmas (not exploitative yet)

### Session Layer
- SSL/TLS handshake overview
- RDP, SMB session creation

### Presentation Layer
- Data transformation: ASCII vs Unicode
- SSL/TLS encryption examples

### Application Layer
- HTTP headers: Host, Cookie, User-Agent
- DNS record types: A, AAAA, CNAME, MX, TXT
- DHCP options and packet flow (DORA)
- FTP active vs passive mode
- SMTP, IMAP, POP3 comparison
