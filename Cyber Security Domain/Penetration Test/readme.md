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


### 🧭 Attack Flow (Mermaid Diagram)

```mermaid
flowchart TD
    A[Initial Access] --> B[External Recon (OSINT, Shodan)]
    B --> C[Port & Service Scanning (Nmap, Masscan)]
    C --> D[Vulnerability Scanning (CVE, Nuclei, Nessus)]
    D --> E[Exploitation (T1190, T1078, Public Exploits)]
    E --> F[Internal Foothold / VPN Entry / LAN Access]

    F --> G[Internal Recon (BloodHound, SMB, ARP)]
    G --> H[Credential Dumping (Mimikatz, procdump)]
    H --> I[Lateral Movement (T1021: RDP, WinRM, WMI)]
    I --> J[Privilege Escalation (T1068, misconfigs)]
    J --> K[Persistence (Scheduled Tasks, Registry)]
    K --> L[Data Exfiltration (DNS, HTTP)]
    L --> M[Cleanup & Anti-Forensics]

    subgraph MITRE Mapping
        E
        H
        I
        J
    end
```
