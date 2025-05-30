## 🧷 Hardware Penetration Testing

### 🧭 Introduction to Hardware Hacking
- **What is hardware penetration testing?**
- **Goals**: data extraction, bypass protections, physical compromise  
- **Typical targets**: routers, IoT, embedded devices, ATMs, POS  
- **Legal and ethical considerations**  
- **Required lab equipment and safety guidelines**

### 🔌 Physical Interface Discovery & Access
- Identifying debugging interfaces: UART, JTAG, SPI, I2C  
- Locating test points and headers using multimeter, logic analyzer  
- Pinout mapping:
  - Multimeter (continuity check)
  - [Saleae Logic Analyzer](https://www.saleae.com/)
  - [Bus Pirate](http://dangerousprototypes.com/docs/Bus_Pirate)
- Interfacing tools:
  - [FTDI](https://www.ftdichip.com/), [CP2102 USB-TTL](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
  - [CH341A Programmer](https://github.com/neatzsche/CH341A-programmer)
  - [JTAGulator](https://www.grandideastudio.com/jtagulator/)
  - [OpenOCD](http://openocd.org/)
- Chip-off techniques using hot air station (e.g., [Hakko FX-888D](https://www.hakko.com/english/products/hakko_fx888d.html))

### 📡 RF and Wireless Communication Analysis
- Protocols: Bluetooth, BLE, Zigbee, LoRa, Sub-GHz, NFC, RFID  
- Tools:
  - [HackRF One](https://greatscottgadgets.com/hackrf/)
  - [RTL-SDR](https://www.rtl-sdr.com/)
  - [LimeSDR](https://limemicro.com/products/boards/limesdr/)
  - [Universal Radio Hacker](https://github.com/jopohl/urh)
  - [GQRX](https://gqrx.dk/)
  - [BTLEJack](https://github.com/virtualabs/btlejack)
  - [KillerBee](https://github.com/riverloopsec/killerbee)
  - [Proxmark3](https://github.com/Proxmark/proxmark3)

### 📦 Flipper Zero & Sub-GHz Attacks
- **[Flipper Zero](https://flipperzero.one/)**: versatile portable hacker tool
  - Supports Sub-GHz (300-928 MHz), RFID, NFC, IR, iButton, GPIO
  - Add custom firmware: [RogueMaster Firmware](https://github.com/RogueMaster/FlipperZero-firmware)
- Use cases:
  - Replay Sub-GHz signals (e.g., car fobs, remote switches)
  - NFC badge sniffing, iButton spoofing, infrared replay
- Sub-GHz bands:
  - 315 MHz (US), 433 MHz (EU), 868 MHz (LoRa), 915 MHz (Americas)

### 🧲 Faraday Cages & RF Isolation
- **Faraday cage**: metal mesh enclosure that blocks external EM signals
- Uses:
  - Prevent signal leakage during testing
  - Create interference-free RF testing zone
- DIY:
  - RF shield bags, copper mesh, foil-lined containers
- Testing:
  - Use SDR to monitor if signal leaks out
- 📎 Reference: [Faraday Box DIY Guide](https://www.rfexplorer.com/faraday/)

### 🔭 Reconnaissance via FCC ID
- Search device's **FCC ID** (usually printed on back) at [https://fccid.io](https://fccid.io)
  - Access internal photos, teardown docs, RF emissions specs
  - Identify chipsets and antennas in use
- Example: [https://fccid.io/2ARCU-FZ](https://fccid.io/2ARCU-FZ) (Flipper Zero)

### 💾 Firmware Extraction & Analysis
- Dumping flash chips (SPI, NAND, NOR):
  - [CH341A Programmer](https://github.com/neatzsche/CH341A-programmer)
  - SOIC-8 Clip, Bus Pirate
- Tools:
  - [binwalk](https://github.com/ReFirmLabs/binwalk)
  - [Firmware-Mod-Kit](https://github.com/mirror/firmware-mod-kit)
  - [Ghidra](https://ghidra-sre.org/)
  - [Cutter](https://cutter.re/)
  - [QEMU](https://www.qemu.org/)
- Tasks:
  - Extract squashfs, cramfs
  - Identify credentials, API keys, certificates

### 🧠 Reverse Engineering & Debugging
- Microcontroller identification (e.g., STM32, ESP32, NXP)
- Resources:
  - [Datasheet Archive](https://www.datasheetarchive.com/)
  - [All About Circuits](https://www.allaboutcircuits.com/)
- Debugging:
  - [IDA Pro](https://hex-rays.com/ida-pro/)
  - [Ghidra](https://ghidra-sre.org/)
  - Emulation with QEMU or Unicorn

### 🔐 Bypassing Protections
- UART login bypass (e.g., interrupt boot and get root shell)
- U-Boot tricks: `printenv`, `setenv`, `bootd`
- Logic flaws in update mechanism (unauthenticated updates)
- Modify NAND/NOR to reset password or insert backdoor

### ⚡ Glitching Attacks (Fault Injection)
- Techniques:
  - Voltage glitching (e.g., ChipWhisperer)
  - Clock glitching
  - EM pulse injection
- Goals:
  - Bypass secure boot, authentication routines
  - Unlock debug features
- Tools:
  - [ChipWhisperer](https://chipwhisperer.io/)
  - [GlitchKit](https://glitchkit.io/)
  - [CrowbarD](https://github.com/newaetech/crowbar-d)
- 🎥 [Voltage Glitching Demo](https://www.youtube.com/watch?v=wWfwoM6zI8U)

### 🧪 Recommended Lab Equipment
- **Basic**:
  - [Hakko Soldering Station](https://www.hakko.com/)
  - Hot air rework station (e.g., Quick 861DW)
  - Antistatic mat & strap
- **Debugging**:
  - [Saleae Logic](https://www.saleae.com/)
  - [Bus Pirate](http://dangerousprototypes.com/docs/Bus_Pirate)
  - USB analyzers (e.g., Beagle)
- **Wireless**:
  - [Flipper Zero](https://flipperzero.one/)
  - [HackRF One](https://greatscottgadgets.com/hackrf/)
  - [Proxmark3](https://github.com/Proxmark/proxmark3)

### 🔁 Methodical Testing Workflow
1. **Scoping**: Define objectives and legal boundaries  
2. **Recon**:
   - Photos, model info, FCC ID search
   - Disassembly and documentation
3. **Interface Discovery**:
   - Locate UART/SPI/JTAG/I2C
4. **Firmware Extraction**:
   - Dump flash using SOIC clip / CH341A
5. **Static Analysis**:
   - Use binwalk, strings, Ghidra
6. **Dynamic Testing**:
   - Glitching, emulation, live UART interaction
7. **Wireless Testing**:
   - Record RF, attempt replay or spoofing
8. **Documentation**

### 🧠 Real-World Scenarios
- UART shell on router reveals root login
- BLE smart lock unlock via replay
- ATM debug port gives access to PIN pad firmware
- RFID key cloning with Proxmark3

### 📋 Reporting & Deliverables
- PCB photos, annotated pinouts
- Firmware hash & binary copy
- Extracted secrets & credentials
- List of vulnerabilities with CVSS scores
- Mitigation advice:
  - Enable secure boot, encrypt flash
  - Fuse burning, disable UART/JTAG in production
  - Harden firmware update logic
