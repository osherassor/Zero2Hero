# 🔍 Digital Forensics & Incident Response (DFIR)

## 🧭 Introduction to DFIR
- Definition and scope of Digital Forensics and Incident Response
- Key differences between forensics and IR
- Use cases: breaches, malware, data leaks, insider threats
- Legal and ethical obligations
- Chain of custody, evidence admissibility, and documentation

---

## 💾 Digital Forensics Fundamentals
- **Sources of evidence**:
  - Memory (RAM)
  - Disks (HDD, SSD)
  - Network (packets, logs)
  - Mobile devices
  - Cloud environments

- **Acquisition Techniques**:
  - Bit-by-bit imaging: `dd`, FTK Imager, Guymager
  - Live acquisition vs dead box forensics
  - Write blockers and bypassing anti-forensics

- **Popular Tools**:
  - [Autopsy](https://www.sleuthkit.org/autopsy/)
  - [FTK](https://accessdata.com/)
  - [EnCase](https://www.guidancesoftware.com/)
  - [X-Ways Forensics](https://www.x-ways.net/)
  - [Volatility](https://github.com/volatilityfoundation)
  - [Sleuth Kit](https://www.sleuthkit.org/)
  - [Plaso (log2timeline)](https://github.com/log2timeline/plaso)

- **File System Analysis**:
  - NTFS, FAT32, EXT4, APFS
  - Deleted file recovery
  - Hidden partitions and artifacts

---

## 🔬 Memory Forensics
- Why RAM matters in incident response
- Acquisition tools:  
  - `winpmem`, `DumpIt`
- Analysis tools:  
  - [Volatility](https://github.com/volatilityfoundation)  
  - [Rekall](https://github.com/google/rekall)

- What can be extracted:
  - Running processes and network connections
  - Loaded DLLs
  - Injected code and malware hooks
  - Credential artifacts (e.g., LSASS)
  - Encryption keys and logs in memory

---

## 🖥️ Disk & File System Analysis
- Metadata and MACB timestamps
- Hidden and slack space analysis
- Alternate Data Streams (ADS)
- File carving techniques
- File signature validation and hash matching (e.g., NSRL, VirusTotal)

---

## 🌐 Network Forensics
- Capturing traffic with `tcpdump`, `Wireshark`
- Protocol analysis (HTTP, DNS, SMB, FTP, TLS)
- Session reconstruction and artifact correlation
- Indicators of exfiltration and C2 communication
- Use of tools: [Arkime](https://arkime.com/), Zeek, Suricata

---

## 📱 Mobile & Cloud Forensics

### 📱 Mobile
- Acquisition types: logical, file system, physical
- Tools: Cellebrite, Magnet AXIOM, MOBILedit
- Extracting chats, GPS, call logs, browser data

### ☁️ Cloud
- Cloud platforms: AWS, Azure, GCP
- Evidence via APIs and audit logs
- Challenges: multi-tenancy, jurisdiction, volatility

---

## 🚨 Incident Response Process

### 1. Preparation
- IR policy, playbooks, escalation matrix
- Logging and alerting configuration
- Communication planning (internal/external)

### 2. Identification
- Detect anomalies via SIEM, EDR, user reports
- IOC collection: hashes, IPs, domains
- Threat triage and validation

### 3. Containment
- Short-term: isolate affected systems
- Long-term: firewall rules, patch rollout

### 4. Eradication
- Malware and backdoor removal
- Vulnerability remediation

### 5. Recovery
- System restoration
- Monitor for reinfection
- Validate business continuity

### 6. Lessons Learned
- RCA (Root Cause Analysis)
- Reporting to stakeholders
- Improving controls and detection rules

---

## 🧪 Incident Types & Use Cases
- Ransomware outbreaks
- Business Email Compromise (BEC)
- Web server exploitation
- Insider threat incidents
- Credential harvesting and reuse
- Supply chain compromise (e.g., SolarWinds)

---

## 🧰 IR Tools

### 🔍 Triage & Collection
- [Velociraptor](https://www.velociraptor.app/)
- [KAPE](https://www.kroll.com/en/insights/publications/cyber/kroll-artifact-parser-extractor-kape)
- GRR Rapid Response

### 🧠 Memory Capture
- DumpIt, WinPMEM

### 🧪 Analysis & Investigation
- Autopsy, [SIFT Workstation](https://digital-forensics.sans.org/community/downloads)
- ELK Stack, Splunk

### 🌐 Threat Intelligence
- VirusTotal, AbuseIPDB, Hybrid Analysis, MISP

---

## 🧠 MITRE ATT&CK & DFIR
- Use ATT&CK for mapping tactics and techniques
- Track TTPs used in incident
- Identify patterns in threat actor behavior
- Integrate into detection playbooks and SIEM rules

---

## 📋 Reporting & Documentation
- Timeline of incident events
- Evidence preservation logs and chain of custody
- IOCs and relevant artifacts
- Executive summary with business impact
- Detailed findings and remediation recommendations
