## 🏭 OT (Operational Technology) Penetration Testing

### 🎯 Objectives
- Assess security posture of industrial control systems (ICS) and SCADA environments
- Identify vulnerable components in OT networks, protocols, and physical interfaces
- Simulate potential impact of cyberattacks on critical infrastructure
- Provide risk-based recommendations without disrupting operations

### 🧭 Understanding OT Environments
- **ICS (Industrial Control Systems)**: Used to monitor and control industrial processes
- **SCADA (Supervisory Control and Data Acquisition)**: Remote control of assets and sensors
- **DCS (Distributed Control Systems)**: On-premise automated control of industrial systems
- **PLC (Programmable Logic Controllers)**: Hardware that interfaces with sensors/actuators

### 🛑 Key Considerations
- **Safety and Uptime are critical** – real-world tests can cause physical damage or disruption
- **Passive over Active** – prefer passive reconnaissance; active tests only in non-production
- **Legacy Protocols** – often lack encryption, authentication (e.g., Modbus, DNP3)
- **Air-Gapped Myth** – many systems believed to be isolated are still reachable

### 📡 Common OT Protocols
- [Modbus](https://modbus.org): Serial and TCP-based industrial control protocol
- [DNP3](https://en.wikipedia.org/wiki/DNP3): Used in power and water utilities
- [PROFINET](https://us.profinet.com/): Ethernet-based automation communication
- [BACnet](https://www.bacnet.org/): Building automation (HVAC, lighting)
- OPC, Ethernet/IP, S7, CAN Bus, and others

### 🔍 Reconnaissance & Mapping
- **Passive Discovery**:
  - Network sniffing with [Wireshark](https://www.wireshark.org/)
  - Asset discovery with [GRASSMARLIN](https://github.com/nsacyber/GRASSMARLIN)
  - Identify hosts, protocols, and communications
- **Active Scanning** (use with extreme caution):
  - [Nmap NSE](https://nmap.org/nsedoc/) scripts for OT protocols
  - Custom tools like `modscan`, `s7scan`, or `PLCscan`
  - Protocol fingerprinting with [zGrab](https://github.com/zmap/zgrab)

### ⚙️ Attack Techniques
- **Unauthenticated Read/Write Access** (e.g., Modbus coil manipulation)
- **Command Injection into PLCs**
- **Replay Attacks** – capturing and replaying control traffic
- **Man-in-the-Middle Attacks** – protocol manipulation in transit
- **Denial-of-Service** – crashing PLCs or disabling operator HMI
- **Default Credentials** – hardcoded accounts in legacy systems

### 🛠 Tools for OT Security Testing
- [GRASSMARLIN](https://github.com/nsacyber/GRASSMARLIN): Passive mapping of ICS networks
- [ModScan / ModPoll](https://www.modbusdriver.com/modpoll.html): Interact with Modbus devices
- [PLCscan](https://github.com/hackercast/PLCscan): Discover and fingerprint PLCs
- [Snap7](http://snap7.sourceforge.net/): Siemens S7 protocol interaction
- [SCADAfence Platform](https://www.scadafence.com/)
- [Wireshark ICS protocol dissectors](https://wiki.wireshark.org/Modbus)

### 🧪 Red Team Scenarios
- **Simulation of External Threat Actor** – entry via IT → OT pivoting
- **Malicious Insider** – USB drop or engineering workstation compromise
- **Protocol Abuse** – sending malicious commands to PLCs
- **Physical Attacks** – tampering with sensors, cables, or interfaces

### 📋 Reporting & Deliverables
- Topology map of the OT network and asset inventory
- Vulnerability matrix by device/protocol
- Screenshots or packet captures of findings
- Proof-of-concept (PoC) for non-disruptive attacks
- Recommendations for:
  - Network segmentation (IT/OT separation)
  - Protocol whitelisting and filtering
  - Access control and hardening
  - Intrusion detection (e.g., [Zeek](https://zeek.org/), [Nozomi Networks](https://www.nozominetworks.com/))
- Risk analysis aligned to impact on **availability**, **safety**, and **integrity**

### 🧠 References & Further Reading
- 🧩 [MITRE ATT&CK for ICS](https://attack.mitre.org/matrices/ics/)
- 🧠 [ICS Top 20 Controls – SANS](https://www.sans.org/white-papers/top-20-critical-controls/)
- 🛡 [CISA ICS Advisories](https://www.cisa.gov/news-events/ics-advisories)
- 📘 Book: _Industrial Cybersecurity_ by Pascal Ackerman
