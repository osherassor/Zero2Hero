# 🛡️ Security Operations Center (SOC)

## 🏢 SOC Fundamentals
- **Purpose and role of a SOC**
- **Types of SOCs**:  
  - Internal SOC  
  - Managed SOC (MSSP)  
  - Hybrid SOC
- **SOC tiers and responsibilities**:  
  - Tier 1: Alert triage, log monitoring  
  - Tier 2: Deep investigation, correlation  
  - Tier 3: Threat hunting, malware analysis  
- **Common roles**:  
  - SOC Analyst (L1/L2)  
  - Incident Responder  
  - SOC Engineer  
  - Threat Hunter  
  - SOC Manager  

---

## 🧰 Core SOC Tools

### 🔹 SIEM – *Security Information and Event Management*
- Use cases: centralized log collection, alerting, dashboards, correlation rules  
- Popular tools:  
  - [Splunk](https://www.splunk.com/)  
  - [IBM QRadar](https://www.ibm.com/products/qradar-siem)  
  - [Microsoft Sentinel](https://azure.microsoft.com/en-us/products/microsoft-sentinel/)  
  - [LogRhythm](https://logrhythm.com/)

### 🔹 SOAR – *Security Orchestration, Automation and Response*
- Automate response playbooks, case management  
- Tools:  
  - [Cortex XSOAR](https://www.paloaltonetworks.com/cortex/xsoar)  
  - [Splunk SOAR](https://www.splunk.com/en_us/software/soar.html)

### 🔹 EDR – *Endpoint Detection and Response*
- Detect and respond to endpoint threats  
- Tools:  
  - [CrowdStrike Falcon](https://www.crowdstrike.com/)  
  - [SentinelOne](https://www.sentinelone.com/)  
  - [VMware Carbon Black](https://www.carbonblack.com/)

### 🔹 IDS/IPS – *Intrusion Detection/Prevention Systems*
- Signature-based vs anomaly-based detection  
- Tools:  
  - [Suricata](https://suricata.io/)  
  - [Snort](https://www.snort.org/)

### 🔹 Threat Intelligence Platforms
- Contextual enrichment, IOC/IOA correlation  
- Examples:  
  - [AlienVault OTX](https://otx.alienvault.com/)  
  - [MISP](https://www.misp-project.org/)  
  - [VirusTotal](https://www.virustotal.com/)

### 🔹 Asset Inventory & Vulnerability Management
- Visibility, scanning, and remediation  
- Tools:  
  - [Qualys](https://www.qualys.com/)  
  - [Tenable Nessus](https://www.tenable.com/products/nessus)  
  - [Rapid7 InsightVM](https://www.rapid7.com/products/insightvm/)

---

## 🔍 Security Monitoring & Detection
- **Key Log Sources**:  
  - Windows Event Logs  
  - Firewall and IDS logs  
  - DNS logs  
  - VPN logs  
  - Proxy/web traffic logs  

- **Detection Techniques**:
  - Use MITRE ATT&CK framework for mapping TTPs  
  - Behavioral analytics (UEBA)  
  - Signature and rule-based detections  
  - Anomaly detection and machine learning models  
  - Tuning and filtering for false positive reduction  
  - Define KPIs (e.g., MTTR, false positive rate, alert volumes)

---

## 🚨 Incident Response Process
1. **Detection and validation**  
2. **Triage and prioritization**  
3. **Containment**
   - Host isolation
   - Credential reset
   - Firewall blocks  
4. **Investigation and RCA (Root Cause Analysis)**  
5. **Eradication and recovery**  
6. **Post-incident review**: lessons learned, reporting, control updates

---

## 🧪 Threat Hunting
- **Hypothesis-driven hunts**: based on threat intel or anomaly signals  
- **Data sources**:  
  - SIEM logs  
  - EDR telemetry  
  - NetFlow / PCAP  
- **Focus on IOAs (Indicators of Attack)** over IOCs  
- **Frameworks**: use [MITRE ATT&CK](https://attack.mitre.org/) for mapping  
- **Techniques**:  
  - PowerShell script analysis  
  - Credential misuse detection  
  - Process injection identification  

---

## 📋 SOC Reporting & Documentation
- Daily shift logs and case notes  
- Full incident timelines  
- Executive summaries  
- Threat landscape and trending reports  
- Analyst KPIs and coverage reports

---

## 🛡️ Blue Team Skills and Challenges
- Log and event analysis  
- Network packet inspection (e.g., Wireshark)  
- Malware triage and sandboxing  
- Memory dump analysis basics  
- Purple Teaming: emulate attacker and test detection  
- Understanding attacker tools and persistence methods  
- Identifying gaps in coverage and improving controls

---

## 🧠 SOC Training & Simulation
- **Lab Environments**:  
  - [DetectionLab](https://github.com/clong/DetectionLab)  
  - [Security Onion](https://securityonionsolutions.com/)  

- **Simulated Attacks & CTFs**:  
  - [Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)  
  - [MITRE Caldera](https://github.com/mitre/caldera)  
  - [MITRE ATT&CK Evaluations](https://attackevals.mitre.org/)  
  - Purple team tabletop exercises  
