# 🛡️ Security Appliances & Defensive Mechanisms

## 🔥 Firewalls (FW)
- **Types of firewalls:**
  - Packet-filtering
  - Stateful inspection
  - Proxy-based (Application Layer)
  - Next-Generation Firewall (NGFW)
- Inbound vs outbound filtering
- Rules and policies (allow/deny, ports, protocols)
- Zone-based firewalling and segmentation
- Logging and alerting
- Integration with SIEM and IPS/IDS

## 🛑 Network Access Control (NAC)
- Purpose: Restrict access based on identity, posture, or location
- 802.1X authentication and RADIUS
- Posture assessment: AV installed, patch level, domain join
- Quarantine VLANs and remediation portals
- Agent-based vs agentless NAC solutions
- Integration with AD, MDM, and threat intelligence

## 🌀 Load Balancers (LB)
- **Types:**
  - L4 (Transport Layer) load balancing
  - L7 (Application Layer) load balancing
- Session persistence (sticky sessions)
- SSL termination vs SSL passthrough
- Health checks and failover
- **Load balancing algorithms:**
  - Round robin
  - Least connections
  - IP hash
- Reverse proxy integration

## 🛡️ Web Application Firewalls (WAF)
- Function: Filter HTTP(S) traffic to/from web apps
- Signature-based vs behavioral WAF
- OWASP Top 10 protections
- **Protection against:**
  - SQL Injection
  - XSS
  - CSRF
  - File inclusion
  - Command injection
- Positive vs negative security models
- **Deployment modes:**
  - Reverse proxy
  - Transparent bridge
  - Inline / Out-of-band
- Cloud-based WAF vs on-prem (e.g., AWS WAF, Cloudflare)

## 🧠 Intrusion Detection / Prevention Systems (IDS/IPS)
- Signature-based vs anomaly-based detection
- Network-based (NIDS) vs host-based (HIDS)
- Inline (IPS) vs passive (IDS)
- Integration with firewall, SIEM, and EDR/XDR
- Common tools: Snort, Suricata, Zeek (Bro)

## 🔍 Endpoint Detection & Response (EDR/XDR)
- Purpose: Monitor, detect, and respond to endpoint threats
- **Features:**
  - Real-time telemetry
  - Behavior-based detection
  - Threat hunting and forensics
  - Automated response actions
- Examples: CrowdStrike, SentinelOne, Microsoft Defender ATP

## 🔄 Security Information and Event Management (SIEM)
- Central logging and event correlation
- Rule-based alerting and dashboards
- Integrations with FW, IDS/IPS, NAC, WAF, etc.
- Log retention and compliance (e.g., PCI-DSS, ISO 27001)
- Threat intelligence feeds and enrichment
- Examples: Splunk, QRadar, ELK Stack, Azure Sentinel

## 🧰 Data Loss Prevention (DLP)
- Monitoring and controlling sensitive data flows
- **Channels:** Email, web, USB, clipboard
- **Detection methods:**
  - Keyword matching
  - Regex
  - Fingerprinting
  - Machine learning-based classification
- Integration with mail servers, proxies, and endpoints

## 📡 Email Security Gateways (SEG)
- Spam filtering, malware scanning, and phishing protection
- DKIM, SPF, DMARC enforcement
- Sandboxing suspicious attachments
- URL rewriting and time-of-click protection

## 🔐 Encryption Gateways / VPN Concentrators
- Secure tunneling for remote access (IPSec, SSL-VPN)
- Site-to-site VPN and remote client VPN
- Authentication mechanisms: Certificates, 2FA, LDAP
- Integration with NAC and SIEM

## ⚙️ Network Packet Brokers (NPB)
- Aggregating and filtering network traffic for monitoring
- Load balancing data to multiple tools
- Packet slicing, masking, and timestamping

## 📦 Deliverables & Insights
- Topology map of security appliance placement
- Policies and configurations review
- Effectiveness analysis per control (e.g., blocked threats, alert volume)
- Gap analysis and architecture improvement suggestions
- Compliance mapping (e.g., ISO, NIST, PCI)
- Recommendations for tuning, upgrades, or redundancy
