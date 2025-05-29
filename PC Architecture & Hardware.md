# 📦 PC Architecture & Hardware

## 🧩 CPU (Central Processing Unit)
- Understand the purpose of the CPU
- Learn about Instruction Cycle: Fetch → Decode → Execute → Write Back
- Explore CPU Components:
  - ALU (Arithmetic Logic Unit)
  - Control Unit
  - Registers (general-purpose, special-purpose)
  - Cache (L1, L2, L3)
- Compare CPU Architectures:
  - x86, x64 (Intel/AMD)
  - ARM architecture
- Concepts of Multi-core and Hyper-Threading
- Clock speed vs performance
- CPU virtualization support (VT-x, AMD-V)
- Power consumption and thermal design
- Tools to monitor CPU usage and temperature

## 📏 RAM (Random Access Memory)
- Understand the purpose of RAM (volatile memory)
- Learn about RAM types:
  - DDR3, DDR4, DDR5
  - ECC vs non-ECC
  - DIMM vs SO-DIMM
- RAM speed (frequency), latency (CL), and channels (single/dual)
- Concepts of paging and swapping
- RAM installation and motherboard compatibility
- How to test RAM stability (e.g., MemTest86)
- RAM vs Virtual Memory
- Overclocking RAM: benefits and risks
- Memory map in OS perspective

## 💽 Storage Devices
- Differentiate between HDD, SSD, NVMe
- Understand storage interfaces:
  - SATA, IDE, M.2, PCIe
- Concept of sectors, blocks, clusters
- TRIM command for SSD
- SMART monitoring
- Disk read/write speeds (IOPS, throughput)
- File storage lifecycle: creation, deletion, recovery
- Defragmentation vs optimization
- Understand boot sectors and partition tables
- Storage benchmarking tools (CrystalDiskMark, HDTune)

## 🧩 Motherboard
- Function of motherboard and chipset
- Form factors: ATX, Micro-ATX, Mini-ITX
- Components:
  - CPU socket
  - RAM slots
  - VRM (Voltage Regulator Modules)
  - CMOS battery
- Buses:
  - Data, Address, Control
  - PCIe lanes and bandwidth
- Chipset functions and models (Intel vs AMD)
- BIOS vs UEFI
- Connectors: SATA, power, USB headers
- Internal vs external connectors
- POST process and beep codes
- Using motherboard manuals for system design

## 🔌 Power Supply Unit (PSU)
- Purpose of PSU in desktop architecture
- Learn about wattage and power budgeting
- Efficiency ratings (80 PLUS Bronze, Gold, Platinum)
- Understand connector types:
  - 24-pin ATX
  - 8-pin CPU
  - PCIe power
  - Molex, SATA power
- Modular vs non-modular PSUs
- Power delivery to GPU, CPU, drives
- PSU protection features: OCP, OVP, SCP
- How to calculate load and headroom
- UPS integration basics
- Tools for monitoring voltage and power draw

## 🔁 Cooling & Thermal Management
- Purpose of cooling in computing
- Passive vs active cooling
- Types of cooling:
  - Air cooling (fans, heatsinks)
  - Liquid cooling (AIO, custom loop)
  - Phase-change cooling (advanced)
- Thermal paste types and application
- Importance of airflow and case design
- Fan curves and noise optimization
- Temperature monitoring tools (HWMonitor, OpenHardwareMonitor)
- BIOS/UEFI fan control settings
- Thermal throttling behavior
- GPU-specific cooling systems

## 🧩 Expansion & Peripherals
- Peripheral connection types:
  - USB (2.0/3.0/3.2/Type-C)
  - Bluetooth, PS/2, Thunderbolt
- Input Devices: keyboard types, mouse DPI, scanners
- Output Devices: monitor refresh rate, printers
- Expansion cards:
  - GPUs, sound cards, capture cards
  - Network cards (Wi-Fi, Ethernet)
- Plug-and-play vs manual driver installs
- IRQ and resource conflict concepts
- Audio subsystems (onboard vs dedicated)
- Display interfaces: VGA, HDMI, DVI, DisplayPort
- BIOS/UEFI settings for peripheral control
- I/O latency considerations

## 🔍 System Building & Troubleshooting
- Choosing compatible components
- POST and troubleshooting boot failures
- Diagnostic LEDs and beeping codes
- Static electricity precautions
- Thermal paste reapplication
- Troubleshooting PSU, RAM, GPU failures
- BIOS resets and firmware updates
- Updating chipset and device drivers
- Interpreting motherboard error codes
- Documentation, schematics, manuals usage
