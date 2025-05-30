
## 📰 OSINT (Open Source Intelligence)

### 🕵️‍♂️ Introduction to OSINT
- Definition and value of OSINT in cybersecurity
- Legal and ethical boundaries
- Difference between passive and active information gathering
- Role in reconnaissance and threat intelligence

### Passive OSINT vs Active OSINT

#### 🟢 Passive OSINT
Passive OSINT involves collecting publicly available data without directly interacting with the target or leaving visible traces. This helps avoid detection and is often used in the early stages of reconnaissance.

- **Local Level (Endpoint):**
  - Reviewing previously downloaded documents for metadata.
  - Analyzing cached data, cookies, or browser history (when obtained legally).
  - Looking at public file metadata (e.g., EXIF in images) already on disk.

- **Network Level:**
  - Monitoring public DNS records without querying the target’s servers.
  - Using passive DNS history tools (e.g., SecurityTrails, PassiveTotal).
  - Viewing SSL certificate transparency logs (e.g., crt.sh) to infer subdomains.

- **Internet Level:**
  - Searching search engines for indexed content (Google Dorking).
  - Reviewing GitHub repos, social media posts, and job boards.
  - Scraping public WHOIS, archive.org snapshots, or pastebin leaks.
  - Monitoring leaked data on breach databases or dark web forums.

#### 🔴 Active OSINT
Active OSINT involves querying, pinging, scanning, or interacting with the target — possibly triggering logs or alerts. It can reveal more detailed info but is riskier in sensitive scenarios.

- **Local Level (Endpoint):**
  - Sending crafted files or links to analyze system behavior or user response.
  - Social engineering through phishing emails that include tracking elements.

- **Network Level:**
  - Performing DNS brute-force or subdomain enumeration.
  - Actively scanning IP ranges using tools like Nmap.
  - Attempting zone transfers (`dig axfr`) or banner grabbing.

- **Internet Level:**
  - Creating decoy LinkedIn or Telegram profiles to engage with employees.
  - Probing S3 buckets or cloud assets directly.
  - Using search APIs with active queries (e.g., Shodan real-time scans)


### 🌎 Data Sources and Surface Levels
- Surface Web: blogs, company websites, public records
- Deep Web: subscription-only resources, academic databases
- Dark Web: Tor-accessible markets, leak sites, forums
- Paste sites (Pastebin, Ghostbin), file sharing platforms
- Code repositories (GitHub, GitLab, Bitbucket)
- Social media platforms: Facebook, LinkedIn, Twitter, TikTok
- Domain registries, WHOIS, DNS records, MX records
- Search engines beyond Google: Yandex, Bing, DuckDuckGo

### ⚖️ OSINT Techniques & Methodologies
- Google dorking (intitle, inurl, filetype, etc.)
- Metadata analysis in images/docs (EXIF, FOCA)
- Subdomain enumeration
- DNS zone transfers and passive DNS analysis
- Email harvesting, breach lookup (haveibeenpwned, dehashed)
- Company structure & employee enumeration (LinkedIn, Hunter.io)
- Git repo leaks and exposed credentials
- Pastebin & Telegram leak tracking
- Threat actor tracking via aliases, PGP keys, reused nicknames

### 🔧 OSINT Tools
- Recon-ng, theHarvester, SpiderFoot, Maltego
- FOCA, Shodan, Censys, ZoomEye, BinaryEdge
- GitRob, truffleHog, GitLeaks
- MetaGoofil, exiftool, pdf-parser.py
- Google Hacking Database (GHDB)
- Social-analyzer, Creepy, Sherlock

### 🌐 Infrastructure Enumeration
- IP address mapping, ASN and BGP lookups
- SSL certificate transparency (crt.sh, censys.io)
- Cloud asset exposure (S3 buckets, Azure blobs)
- IoT search engines (Shodan filters, Censys banners)

### 💼 Use Cases of OSINT
- Pre-engagement reconnaissance in pentests
- Threat intelligence enrichment
- Brand monitoring and executive protection
- Attack surface mapping
- Insider threat detection
- Phishing infrastructure tracking
- Vulnerability disclosure & responsible reporting

### ✉️ Operational Security (OPSEC)
- Protecting analyst identity (VPN, Tor, burner accounts)
- Avoiding search engine fingerprinting
- Decoy traffic and anonymized browsing

### 📝 Reporting OSINT Findings
- Structuring OSINT results: who, what, when, how
- Correlating findings to targets (companies or individuals)
- Annotating timelines and relationships
- Visualizing intel with graphs (Maltego, SpiderFoot, custom tooling)
- Redacting sensitive or unnecessary personal data
