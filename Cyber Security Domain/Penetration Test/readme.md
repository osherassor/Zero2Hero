# 🔍 Penetration Testing

## 🧭 Pentest Lifecycle
- Understanding scope, impact, and goals
- Preparing an effective Rules of Engagement (ROE)
- Gathering legal authorization (get out of jail letter)
- Choosing methodology: PTES, OWASP, NIST SP800-115, custom hybrid
- Environment type: corporate, cloud, hybrid, ICS, IoT
- Reporting expectations, standards, and deliverables

## 🛠 Reconnaissance & OSINT
### Passive Recon:
- WHOIS lookups and domain metadata
- Shodan
- DNS enumeration (AXFR, zone transfers, subdomain brute-force)
- Google dorking and advanced search operators
- Metadata extraction from files (e.g. exiftool, PDFid)
- Social media profiling, LinkedIn scraping, name generation tools
- Certificate transparency search (crt.sh, censys.io)

### Active Recon:
- Ping sweeps, traceroute, TTL analysis
- Port scanning (Nmap, Masscan, Unicornscan)
- Service detection and versioning (banner grabbing, Nmap scripts)
- Network topology fingerprinting

### Tool Arsenal:
- theHarvester, SpiderFoot, Maltego, Amass, FOCA, DNSdumpster
- GitHub & GitLab dorking tools, Shodan, BinaryEdge

## 🌐 Scanning & Enumeration
- Host discovery and network segmentation mapping

### Service enumeration:
- SMB (Enum4linux, smbclient, CrackMapExec, rpcclient)
- SNMP (snmpwalk, onesixtyone)
- LDAP, RDP, FTP, HTTP, DNS, SIP, SMTP, etc.

### Web Enumeration:
- Hidden files/folders (dirsearch, gobuster, ffuf)
- Fingerprinting (whatweb, builtwith, wafw00f)
- Favicon hash matching, JS file analysis, robots.txt

### Vulnerability Scanning:
- Nessus, OpenVAS, Qualys, Nexpose
- Nikto, Nuclei, Burp Suite active/passive scans

## 🔓 Exploitation Techniques

### Credential attacks:
- Bruteforce (Hydra, Medusa, Patator)
- Password spraying, hash cracking (John, Hashcat)
- Kerberoasting, AS-REP Roasting, Pass-the-Hash

### Web exploitation:
- Injection types (SQLi, XSS, XML, command, LDAP, SSTI)
- SSRF, CSRF, IDOR, Open Redirect, HTTP Smuggling
- File inclusion and upload abuses (LFI, RFI)
- CORS misconfiguration, JWT manipulation, path traversal

### CMS vulnerabilities:
- WordPress, Joomla, Drupal modules/themes/plugins
- Exploitation via WPScan, droopescan, wpscan + metasploit

### Binary exploitation (basics):
- Buffer overflow, ROP chains, shellcode injection
- SEH overwrite, egghunting, exploit dev frameworks

### Toolkits:
- Metasploit, Empire, Covenant, Cobalt Strike (demo only)
- Custom payloads with msfvenom, Veil-Evasion, Donut
- Antivirus evasion basics (obfuscation, packing, crypters)

## 📦 Post-Exploitation

### Local enumeration:
- OS info, processes, services, startup tasks
- Installed software, environment variables
- Scheduled tasks, WMI events, registry autoruns

### Privilege Escalation:
- Windows: AlwaysInstallElevated, unquoted paths, DLL hijacking
- Linux: sudo misconfigs, SUID binaries, PATH manipulation
- Tools: winPEAS, LinPEAS, BeRoot, PowerUp, GTFObins

### Credential harvesting:
- Dumping LSASS (Mimikatz, procdump, nanodump)
- secretsdump.py, LaZagne, browser credential storage

### Lateral Movement:
- RDP, PSExec, WMI, DCOM, SMB shares, Token impersonation
- Domain escalation via DCsync, DCSHADOW, delegation abuse

### Persistence:
- Scheduled tasks, startup folders, registry, WMI, services
- Golden Ticket, Silver Ticket, skeleton key techniques

### Data exfiltration, evasion, and cleanup:
- Encoding, staging, chunking (DNS, HTTP, FTP)
- Anti-forensics: timestomping, log wiping, clearing prefetch

## 📃 Reporting & Deliverables
- Executive summaries tailored to business/management
- Technical details with reproduction steps
- Proof-of-Concepts (PoCs) with screenshots
- Risk ratings (CVSSv3, business impact assessment)
- Remediation advice: short-term vs long-term
- Mapping to frameworks: MITRE ATT&CK, OWASP Top 10
- Optional appendices: tool outputs, full logs, hashes
- Communication strategies: email, in-person briefings, PDF/interactive reports

## 🕸 OWASP Top 10 & Web Application Security

- Overview of OWASP organization and community projects
- OWASP Testing Guide v4 methodology
- OWASP Top 10 (latest version)
  - A01: Broken Access Control
  - A02: Cryptographic Failures
  - A03: Injection
  - A04: Insecure Design
  - A05: Security Misconfiguration
  - A06: Vulnerable and Outdated Components
  - A07: Identification and Authentication Failures
  - A08: Software and Data Integrity Failures
  - A09: Security Logging and Monitoring Failures
  - A10: Server-Side Request Forgery (SSRF)
- Manual testing vs automated testing
- Testing tools:
  - Burp Suite Professional (manual + extensions)
  - ZAP Proxy
  - Nikto, dirsearch, ffuf, nuclei
  - Browser developer tools and proxying
- Exploitation techniques per category
- Real-world case studies (e.g., Capital One SSRF, Equifax SQLi)
- Secure coding countermeasures for each OWASP Top 10 category
- Mapping to CWE IDs, MITRE ATT&CK techniques, and compliance requirements


## 🛠️ Penetration Testing Topics Overview

| Penetration Test Type | Subjects |
|-----------------------|----------|
| [Web Application Penetration Testing](./Web%20Application%20Penetration%20Testing) | - Reconnaissance <br> - Authentication <br> - Input Injection <br> - Business Logic <br> - File Uploads <br> - Session Management <br> - API Security <br> - Deployment Issues <br> - OWASP Top 10 |
| [Mobile Application Penetration Testing](./Mobile%20Application%20Penetration%20Testing) | - Static & Dynamic Analysis <br> - Business Logic <br> - Local Storage <br> - Communication Security <br> - OWASP Mobile Top 10 <br> - Reverse Engineering |
| [Thick Client Application Penetration Testing](./Thick%20Client%20Application%20Penetration%20Testing) | - Static/Dynamic Analysis <br> - Business Logic Testing <br> - Reverse Engineering <br> - Authentication <br> - File System and Network Traffic |
| [Internal & External Infrastructure Pentesting (with MITRE Mapping)](./Internal%20%26%20External%20Infrastructure%20Pentesting%20%28with%20MITRE%20Mapping%29) | - External Recon & Exploitation <br> - Internal Enumeration <br> - Privilege Escalation <br> - Lateral Movement <br> - Deliverables |
| [Cloud Penetration Testing](./Cloud%20Penetration%20Testing) | - IAM Misconfigurations <br> - Storage Exposure <br> - Service-Specific Exploits <br> - Post-Exploitation <br> - Containers <br> - Logging Evasion |
| [Radio Frequancy Penetration Test](./Radio%20Frequancy%20Penetration%20Test) | - RF Fundamentals <br> - Reconnaissance <br> - Replay & MiTM Attacks <br> - BLE/Zigbee/NFC Testing <br> - Flipper Zero <br> - Faraday Cage <br> - FCC ID Recon |
| [Hardware Penetration Testing](./Hardware%20Penetration%20Testing) | - Interface Discovery <br> - Firmware Extraction <br> - Reverse Engineering <br> - Protection Bypass <br> - Glitching <br> - Real-World Attacks |
| [OT (Operational Technology) Penetration Testing](./OT%20%28Operational%20Technology%29%20Penetration%20Testing) | - ICS Protocols <br> - SCADA Systems <br> - Purdue Model <br> - Physical Interface Testing <br> - OT Threat Modeling |


