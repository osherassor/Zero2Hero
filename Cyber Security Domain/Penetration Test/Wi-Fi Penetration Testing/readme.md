## 📡 Wi-Fi Penetration Testing

### 🔍 Objective
- Identify and exploit security weaknesses in wireless networks
- Evaluate segmentation, authentication, and encryption practices
- Assess the ability to pivot from wireless to internal networks

### 🧱 Foundational Concepts
- **Wi-Fi Standards**: IEEE 802.11a/b/g/n/ac/ax (Wi-Fi 6, 6E)
- **Frequency Bands**: 2.4 GHz (crowded, long range), 5 GHz (less interference), 6 GHz (Wi-Fi 6E)
- **Modulation**: OFDM (modern), DSSS (legacy)
- **Channel Planning**: Overlapping vs non-overlapping channels, channel hopping
- **Coverage**: Signal strength, AP placement, attenuation

### 🔒 Security Protocols
- **WEP**: Deprecated, crackable in minutes
- **WPA/WPA2-Personal**: PSK-based, susceptible to handshake capture and offline brute-force
- **WPA3-Personal**: SAE handshake, mitigates offline dictionary attacks
- **WPA/WPA2/WPA3-Enterprise**: Uses 802.1X (EAP over RADIUS)
- **EAP Methods**:
  - EAP-TLS (certificate-based, secure)
  - PEAP (MSCHAPv2, crackable)
  - EAP-TTLS
- **PMF**: Protected Management Frames – mitigates deauth/disassoc attacks

### 🛠 Tools & Setup
- **Wireless NIC** with monitor mode & injection support (e.g., Alfa AWUS036ACH)
- **OS**: Kali Linux or Parrot OS
- **Discovery & Capture**:
  - [Airodump-ng](https://www.aircrack-ng.org/)
  - [Kismet](https://kismetwireless.net/)
- **Attack Tools**:
  - [Aircrack-ng](https://www.aircrack-ng.org/)
  - [Bettercap](https://www.bettercap.org/)
  - [hcxdumptool](https://github.com/ZerBea/hcxdumptool) + [hashcat](https://hashcat.net/hashcat/)
  - [eaphammer](https://github.com/s0lst1c3/eaphammer)
  - [Wireshark](https://www.wireshark.org/)
- **Hardware Add-ons**:
  - Wi-Fi Pineapple (client-side phishing / rogue APs)
  - LAN Turtle (pivoting)

### 🧪 Reconnaissance Phase
- Scan for APs: SSID, BSSID, channel, encryption, clients
- Capture beacon frames, probe requests, auth/assoc handshakes
- Identify unprotected or poorly configured APs

### 🎯 Attack Scenarios
- **WPA/WPA2-PSK**:
  - Capture 4-way handshake
  - Crack with dictionary/rainbow tables
- **Deauthentication Attack**:
  - Kick client to force handshake re-authentication
- **PMKID Hash Extraction**:
  - No need for client deauth (faster handshake-less cracking)
- **Rogue AP / Evil Twin**:
  - Clone SSID, lure clients
  - Host malicious login portal (captive portal phishing)
- **Karma Attack**:
  - Auto-respond to probe requests with spoofed APs
- **EAP Downgrade Attack**:
  - Force downgrade to insecure PEAP/MD5 from TLS

### ⚙️ Enterprise Network Attacks
- **MSCHAPv2 Capture**:
  - Rogue AP (PEAP) + credential harvesting
- **NTLM Cracking**:
  - Use `asleap`, `hashcat`, or relay to [Responder](https://github.com/lgandx/Responder)
- **Credential Relay / Pivot**:
  - Access internal resources with relayed enterprise creds (Kerberoasting, SMB relay)

### 🧱 Infrastructure Assessment
- Open SSIDs, dual-mode APs (open + secure)
- Clients leaking probe requests
- Segmentation tests:
  - Is client-to-client traffic allowed?
  - Can clients reach internal LAN?
- Hidden SSID enumeration via probe responses

### 🧾 Deliverables
- 📍 Topology map of APs, clients, encryption methods
- 🧾 Captured handshakes, PMKID hashes, EAP credentials
- 📸 Screenshots of deauth, rogue portals, cracked PSKs
- 🔓 List of discovered vulnerabilities with severity
- 🔧 Recommendations:
  - Strong PSKs or 802.1X
  - Client isolation
  - Disable WPS
  - Enable PMF
  - Use detection systems (WIDS/WIPS)

### 🔗 References & Resources
- [Aircrack-ng Documentation](https://www.aircrack-ng.org/doku.php)
- [OWASP Wireless Testing Guide](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/10-Testing-for-WiFi-Security.html)
- [Wi-Fi Alliance Security Overview](https://www.wi-fi.org/discover-wi-fi/security)
- [hcxdumptool + PMKID attack explanation](https://hashcat.net/forum/thread-7717.html)


---

### 📊 Attack Flow Diagram: WPA2 Handshake Capture & Crack

```mermaid
sequenceDiagram
    participant Attacker as Attacker (Kali)
    participant AP as Access Point (WPA2)
    participant Client as Victim Device

    Note over Attacker: Monitor mode enabled
    Attacker->>AP: Listen for beacon frames
    Attacker->>Client: Deauthentication frame (spoofed)
    Client-->>AP: Reconnect & start 4-way handshake
    AP-->>Client: ANonce
    Client-->>AP: SNonce + MIC
    Note right of Attacker: Captures handshake
    Attacker->>Attacker: Run hashcat on handshake
    Attacker->>Attacker: Brute-force PSK