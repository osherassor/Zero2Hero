## 📻 RF (Radio Frequency) Security Testing

### 🎯 Objective
- Assess and exploit vulnerabilities in RF-based technologies (beyond Wi-Fi)  
- Evaluate custom protocols, hardware transmissions, and security mechanisms

---

### 🧠 Fundamentals of RF Communication
- Analog vs Digital Signals  
- Frequency Spectrum: LF, HF, VHF, UHF, ISM bands  
- Modulation Types: AM, FM, ASK, FSK, PSK, GFSK  
- Bandwidth, latency, and signal-to-noise ratio  
- Channel separation and interference considerations

---

### 📡 Common RF Technologies
- Bluetooth & BLE  
- Zigbee & Z-Wave  
- LoRa & LoRaWAN  
- RFID & NFC  
- Proprietary RF remotes and sensors (e.g., car fobs, alarms)  
- Satellite and radio broadcast

---

### 🛠 Hardware and Tools
- **Software Defined Radio (SDR)**: HackRF One, RTL-SDR, USRP  
- **Antennas**: directional, omnidirectional, Yagi  
- **Flipper Zero**: for Sub-GHz signal capture, replay, and signal analysis  
- **Signal Isolation**: using Faraday cages for controlled environments  
- RF analyzers: GQRX, SDR#, GNURadio, URH  
- Protocol-specific tools:
  - BTLEJack (BLE), KillerBee (Zigbee), Proxmark3 (RFID), YardStick One (Sub-GHz)

---

### 🧪 Signal Isolation: Faraday Cage
A **Faraday Cage** is an enclosure made of conductive material (e.g., metal mesh or foil) used to **block electromagnetic fields**. In RF testing:
- It isolates devices to **prevent unintended leakage** or interference  
- Ideal for safe replay attacks, fuzzing, or sniffing without disturbing other systems  
- Portable RF isolation bags can be used for quick field analysis

> 🔗 [Wikipedia: Faraday Cage](https://en.wikipedia.org/wiki/Faraday_cage)

---

### 🛰 Reconnaissance and Signal Discovery

#### 🔍 RF Recon Process (S.M.B.I.R.)
A practical methodology for RF analysis:

**S**niff → **M**atch → **B**reak → **I**nject → **R**eplay

1. **Sniff**: Use tools like GQRX, SDR#, URH, or Flipper Zero to detect active frequencies  
2. **Match**: Analyze modulation and patterns to match known protocols  
3. **Break**: Reverse or decode signal contents (e.g., button codes, authentication sequences)  
4. **Inject**: Craft custom signals or modify existing ones  
5. **Replay**: Transmit saved signals to test control or bypass

#### 🧠 What Can You Learn from an FCC ID?
Any RF device sold legally in the U.S. has a printed `FCC ID` that leads to **schematics, photos, antenna specs, and test results**. You can:

- Identify chipset (e.g., CC1101, nRF24L01)  
- Discover exact frequency ranges used  
- Get internal photos for antenna analysis  
- Use it to pick the right SDR setup

> 🔗 [FCC ID Search Tool](https://fccid.io/)

---

### 🧪 Attack Techniques
- **Replay attacks** on unencrypted Sub-GHz devices (garage doors, car fobs)  
- **Signal jamming** of target frequencies (e.g., 433 MHz, 868 MHz)  
- **BLE/Zigbee MitM** using rogue devices  
- **Brute-forcing** RF commands with signal fuzzers  
- **Proprietary Protocol Abuse**: many vendors use simple encoding without security

---

### 🧱 Specialized Scenarios
- NFC payment spoofing with Proxmark3  
- LoRaWAN Join Accept replay or key misuse  
- BLE spoofing with BTLEJack (identity spoof or passive sniffing)  
- Zigbee command injection with KillerBee  
- RF ID cloning and relay with Flipper or Proxmark3

---

### 📦 Flipper Zero and Sub-GHz
**Flipper Zero** can:
- Capture, analyze and replay RF signals from common key fobs and remotes  
- Brute-force rolling code systems (limited support)  
- Read and clone NFC, RFID, and IR  
- Work in offline environments and assist with portable testing

> 🔗 [Flipper Zero Sub-GHz Docs](https://docs.flipperzero.one/sub-ghz)  
> 🔗 [Awesome Flipper Zero Tools](https://github.com/djsime1/awesome-flipperzero)

---

### 📚 References and Further Reading
- 📘 [Universal Radio Hacker (URH)](https://github.com/jopohl/urh)  
- 📘 [Great Scott Gadgets – HackRF](https://greatscottgadgets.com/hackrf/)  
- 📘 [SDR# (SDRSharp)](https://airspy.com/download/)  
- 📘 [FCC ID Lookup](https://fccid.io)  
- 📘 [RTL-SDR Getting Started](https://www.rtl-sdr.com/rtl-sdr-quick-start-guide/)  
- 📘 [Proxmark3 RFID Toolkit](https://github.com/Proxmark/proxmark3)

---

### 📦 Deliverables
- RF device map: technology, frequency, encryption  
- Captured transmissions (raw and decoded formats)  
- Screenshots of spectrum analysis and signal manipulation  
- Security gaps in protocol/firmware implementations  
- Recommendations for signal filtering, protocol encryption, shielding  
- Faraday cage test logs, environment isolation report
