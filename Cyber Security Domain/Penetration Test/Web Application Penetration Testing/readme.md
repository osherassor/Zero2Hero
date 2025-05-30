# 🌐 Web Application Penetration Testing

## 🎯 Objectives & Scope
- Identify and exploit vulnerabilities in web applications.
- Assess authentication, session management, input validation, and access controls.
- Simulate real-world attacker behavior to uncover flaws across the app's attack surface.
- Align with OWASP Testing Guide and OWASP Top 10 risks.

## 🧰 Environment & Tools
- Browsers with extensions (e.g., HackBar, Wappalyzer)
- Intercepting proxies: Burp Suite, OWASP ZAP
- Scanners: [Nuclei](https://github.com/projectdiscovery/nuclei), Nikto, sqlmap, dirsearch, ffuf
- Manual tools: curl, Postman, browser dev tools
- Wordlists: [AwesomeWL – Common_list by Osher Assor](https://github.com/osherassor/AwesomeWL/blob/main/Common_list.txt)
- Scripting: Python, Bash, or JS snippets for custom payloads

## 🧭 Recon & Mapping
- Discover subdomains and endpoints (e.g., with Amass, Subfinder)
- Crawl app to find hidden pages (robots.txt, sitemap.xml)
- Fingerprint technologies and CMS used
- Identify WAF presence and bypass strategies

## 🧪 Input Handling & Injection Attacks
- SQL Injection (Classic, Blind, Time-based)
- XSS (Reflected, Stored, DOM)
- Command Injection
- XML External Entities (XXE)
- Server-Side Template Injection (SSTI)
- Server-Side Request Forgery (SSRF)

## 🔐 Authentication & Authorization Testing
- Brute-force login (Hydra, Burp Intruder)
- Bypass authentication via logic flaws or parameter tampering
- Insecure password reset flows
- Multi-factor authentication bypass techniques
- IDOR and broken object-level authorization
- Vertical and horizontal privilege escalation

## 🧠 Business Logic Testing
- Abuse of trust relationships, workflows, and logic assumptions
- Price manipulation, cart tampering, API misuse
- Abuse of client-side logic

## 💾 File Handling & Uploads
- Upload unrestricted file types
- Content-type evasion
- Path traversal via filenames
- Bypass of extension blacklists and MIME checks

## 📜 Session Management
- Session fixation and token prediction
- Secure cookie flags (HttpOnly, Secure)
- JWT attacks: none alg, key confusion, token replay
- Session timeout and logout bypass

## 📤 Client-Side Vulnerabilities
- JavaScript injection via DOM-based XSS
- CSP bypasses
- Clickjacking
- CORS misconfiguration

## ⚙️ APIs & Backend Interaction
- Testing REST, GraphQL, and SOAP endpoints
- Missing or weak authentication
- Mass assignment and insecure deserialization
- Parameter pollution and tampering

## 📦 Deployment & Configuration Issues
- Information leakage (error messages, headers, comments)
- Default credentials or test accounts
- Directory listing
- Debug endpoints and admin panels
- Improper cache control

## 📊 Mapping to OWASP Top 10 (2021)
- A01: Broken Access Control
- A02: Cryptographic Failures
- A03: Injection
- A04: Insecure Design
- A05: Security Misconfiguration
- A06: Vulnerable & Outdated Components
- A07: Identification & Authentication Failures
- A08: Software & Data Integrity Failures
- A09: Security Logging & Monitoring Failures
- A10: Server-Side Request Forgery (SSRF)

## 🧾 Deliverables
- Executive summary and business impact
- Proof-of-concept for each vulnerability
- Reproduction steps and screenshots
- Remediation guidance (short and long-term)
- Risk rating: CVSS, OWASP mapping, severity matrix
- Optional appendix with tool outputs and logs

## 📚 References
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Top 10 (2021)](https://owasp.org/www-project-top-ten/)
- [Burp Suite Documentation](https://portswigger.net/burp/documentation)
- [PayloadAllTheThings GitHub](https://github.com/swisskyrepo/PayloadsAllTheThings)
- [ProjectDiscovery GitHub (Nuclei, Subfinder, etc.)](https://github.com/projectdiscovery)
- [AwesomeWL – Common_list by Osher Assor](https://github.com/osherassor/AwesomeWL/blob/main/Common_list.txt)
