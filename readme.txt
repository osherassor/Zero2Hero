📘 About This Document – A Personal Note

As someone deeply rooted in the world of cybersecurity, I believe that true expertise doesn’t start with tools or exploits — it starts with foundations. Cybersecurity is built on understanding: how operating systems work, how memory is managed, how a packet flows through a network, how code interacts with hardware. Only when these principles are mastered can we begin to think like attackers, defenders, architects, or investigators.

This document is much more than a syllabus. It’s a personal roadmap — a structured path I’ve built out of the belief that anyone entering cybersecurity should first master the core building blocks before diving into specialized roles. For me, the essence of real cybersecurity is not superficial knowledge, but depth, clarity, and long-term growth.

In my opinion, one of the most important values in cybersecurity is the ability to learn independently. Every concept or keyword in this document can — and should — be further explored using tools like Google, YouTube, or AI-based assistants. This isn’t a textbook. It’s a map. And it’s up to the learner to explore each path, dig deeper, and truly own their learning process.

The first part of this syllabus covers everything I believe should be learned before touching cybersecurity itself — the technical DNA behind the discipline. The second part dives into the core domains of cybersecurity, such as penetration testing, threat modeling, secure development, GRC, DFIR, and more — each with detailed, actionable learning objectives.

💬 If you have additional suggestions, corrections, or would like to contribute videos, tutorials, or structured guides aligned with any section of this document, feel free to reach out directly. Collaboration is welcome.

This is a living project — evolving as technology, threats, and roles evolve. I hope it helps light the path for anyone serious about mastering cybersecurity.

— Osher Assor


📦 PC Architecture & Hardware
    •	🧩 CPU (Central Processing Unit)
        o	Understand the purpose of the CPU
        o	Learn about Instruction Cycle: Fetch → Decode → Execute → Write Back
        o	Explore CPU Components:
            o	ALU (Arithmetic Logic Unit)
            o	Control Unit
            o	Registers (general-purpose, special-purpose)
            o	Cache (L1, L2, L3)
        o	Compare CPU Architectures:
            o	x86, x64 (Intel/AMD)
            o	ARM architecture
        o	Concepts of Multi-core and Hyper-Threading
        o	Clock speed vs performance
        o	CPU virtualization support (VT-x, AMD-V)
        o	Power consumption and thermal design
        o	Tools to monitor CPU usage and temperature
    •	📏 RAM (Random Access Memory)
        o	Understand the purpose of RAM (volatile memory)
        o	Learn about RAM types:
            o	DDR3, DDR4, DDR5
            o	ECC vs non-ECC
            o	DIMM vs SO-DIMM
        o	RAM speed (frequency), latency (CL), and channels (single/dual)
        o	Concepts of paging and swapping
        o	RAM installation and motherboard compatibility
        o	How to test RAM stability (e.g., MemTest86)
        o	RAM vs Virtual Memory
        o	Overclocking RAM: benefits and risks
        o	Memory map in OS perspective
    •	💽 Storage Devices
        o	Differentiate between HDD, SSD, NVMe
        o	Understand storage interfaces:
            o	SATA, IDE, M.2, PCIe
        o	Concept of sectors, blocks, clusters
        o	TRIM command for SSD
        o	SMART monitoring
        o	Disk read/write speeds (IOPS, throughput)
        o	File storage lifecycle: creation, deletion, recovery
        o	Defragmentation vs optimization
        o	Understand boot sectors and partition tables
        o	Storage benchmarking tools (CrystalDiskMark, HDTune)
    •	🧩 Motherboard
        o	Function of motherboard and chipset
        o	Form factors: ATX, Micro-ATX, Mini-ITX
        o	Components:
            o	CPU socket
            o	RAM slots
            o	VRM (Voltage Regulator Modules)
            o	CMOS battery
        o	Buses:
            o	Data, Address, Control
            o	PCIe lanes and bandwidth
        o	Chipset functions and models (Intel vs AMD)
        o	BIOS vs UEFI
        o	Connectors: SATA, power, USB headers
        o	Internal vs external connectors
        o	POST process and beep codes
        o	Using motherboard manuals for system design
    •	🔌 Power Supply Unit (PSU)
        o	Purpose of PSU in desktop architecture
        o	Learn about wattage and power budgeting
        o	Efficiency ratings (80 PLUS Bronze, Gold, Platinum)
        o	Understand connector types:
            o	24-pin ATX
            o	8-pin CPU
            o	PCIe power
            o	Molex, SATA power
        o	Modular vs non-modular PSUs
        o	Power delivery to GPU, CPU, drives
        o	PSU protection features: OCP, OVP, SCP
        o	How to calculate load and headroom
        o	UPS integration basics
        o	Tools for monitoring voltage and power draw
    •	🔁 Cooling & Thermal Management
        o	Purpose of cooling in computing
        o	Passive vs active cooling
        o	Types of cooling:
            o	Air cooling (fans, heatsinks)
            o	Liquid cooling (AIO, custom loop)
            o	Phase-change cooling (advanced)
        o	Thermal paste types and application
        o	Importance of airflow and case design
        o	Fan curves and noise optimization
        o	Temperature monitoring tools (HWMonitor, OpenHardwareMonitor)
        o	BIOS/UEFI fan control settings
        o	Thermal throttling behavior
        o	GPU-specific cooling systems
    •	🧩 Expansion & Peripherals
        o	Peripheral connection types:
            o	USB (2.0/3.0/3.2/Type-C)
            o	Bluetooth, PS/2, Thunderbolt
        o	Input Devices: keyboard types, mouse DPI, scanners
        o	Output Devices: monitor refresh rate, printers
        o	Expansion cards:
            o	GPUs, sound cards, capture cards
            o	Network cards (Wi-Fi, Ethernet)
        o	Plug-and-play vs manual driver installs
        o	IRQ and resource conflict concepts
        o	Audio subsystems (onboard vs dedicated)
        o	Display interfaces: VGA, HDMI, DVI, DisplayPort
        o	BIOS/UEFI settings for peripheral control
        o	I/O latency considerations
    •	🔍 System Building & Troubleshooting
        o	Choosing compatible components
        o	POST and troubleshooting boot failures
        o	Diagnostic LEDs and beeping codes
        o	Static electricity precautions
        o	Thermal paste reapplication
        o	Troubleshooting PSU, RAM, GPU failures
        o	BIOS resets and firmware updates
        o	Updating chipset and device drivers
        o	Interpreting motherboard error codes
        o	Documentation, schematics, manuals usage


🧠 Digital Logic & Binary Systems
    •	💻 Binary Number Systems
        o	What is binary and why computers use it
        o	Base conversions:
            o	Decimal → Binary
            o	Binary → Decimal
            o	Binary → Hexadecimal
        o	Signed vs unsigned numbers
        o	Two's complement
        o	Endianness: little-endian vs big-endian
        o	Floating-point representation (IEEE 754)
        o	Binary arithmetic: addition, subtraction, multiplication
        o	Bitwise operations:
            o	AND, OR, NOT, XOR
            o	Bit shifting (<<, >>)
        o	Bit masking and flag fields
        o	Representing negative numbers and overflows
    •	⚖️ Boolean Algebra & Logic Gates
        o	Boolean variables and logic expressions
        o	Truth tables and logic evaluation
        o	Fundamental logic gates:
            o	AND, OR, NOT
        o	Derived gates:
            o	NAND, NOR, XOR, XNOR
        o	De Morgan's Laws
        o	Combinational logic
        o	Minimizing logic expressions (Karnaugh Maps)
        o	Logic circuit simulation tools
        o	Logic propagation delays
        o	Using Boolean logic in control flow (if/else, conditions)
    •	🛠️ Digital Components
        o	Flip-Flops:
            o	SR, D, JK, T Flip-Flops
        o	Latches vs Flip-Flops
        o	Clocking mechanisms and edge-triggered design
        o	Registers and shift registers
        o	Counters (synchronous, asynchronous)
        o	Timers and clocks
        o	Multiplexers, Demultiplexers
        o	Encoders and Decoders
        o	Comparators
        o	Tri-state buffers
    •	⚖️ Combinational Circuits
        o	Half Adder, Full Adder
        o	Multiplexer / Demultiplexer
        o	Decoder / Encoder
        o	ALU Design (Arithmetic Logic Unit)
        o	Circuit diagrams using logic gate symbols
        o	Simulation with digital logic tools (e.g., Logisim)
        o	Circuit optimization and simplification
    •	🌐 Data Representation & Encoding
        o	ASCII vs Unicode (UTF-8, UTF-16)
        o	Binary-coded decimal (BCD)
        o	Parity bits and error detection
        o	Checksum algorithms
        o	Hamming code (Error correction)
        o	Gray code and its use in hardware
        o	Memory encoding formats
        o	Digital signal encoding concepts (NRZ, Manchester)
        o	Compression basics (lossless vs lossy)
        o	Base64 and hexadecimal in data transmission
    •	🌀 Sequential Logic & FSMs
        o	Difference between combinational and sequential logic
        o	State machines:
            o	Moore vs Mealy models
        o	Designing FSMs:
            o	State diagrams
            o	State transition tables
        o	Applications in digital design
        o	Use in protocol parsing
        o	Timing diagrams and delays
        o	HDL-based implementation (optional advanced)
        o	Clock synchronization
        o	Metastability issues in hardware
    •	🔹 Logic Implementation Tools
        o	Schematic vs text-based design
        o	Digital circuit simulators:
            o	Logisim
            o	CircuitVerse
            o	Digital Works
        o	HDL introduction:
            o	Verilog vs VHDL (basics only)
        o	FPGA basics (field-programmable gate arrays)
        o	Breadboard prototyping (for physical learners)
    •	📊 Digital Measurement & Timing
        o	Measuring signal timings
        o	Clock cycles and frequency
        o	Debouncing signals
        o	Propagation delay
        o	Signal timing diagrams
        o	Synchronizing inputs
        o	Flip-Flop setup/hold time
        o	Logic analyzer use
    •	🥯 Real-world Applications
        o	Use of logic in microprocessors
        o	Control systems
        o	Memory and storage controllers
        o	Network hardware logic paths
        o	Encoders/decoders in multimedia
        o	Sensor signal digitization
        o	Logic in keyboard/mouse controllers
        o	Use in IoT device design
        o	Error detection in communication protocols


🖥️ Operating System Fundamentals
        •	🧱 What is an Operating System?
        o	Define OS as a mediator between hardware and applications
        o	Key responsibilities: resource management, UI, hardware abstraction
        o	History: batch processing → time sharing → graphical OS
        o	Real-time vs general-purpose OS
        o	Embedded vs desktop vs server OS
        o	Monolithic vs microkernel design
        o	Overview of major OS families (Windows, UNIX/Linux, macOS)
        o	Multitasking, multiprocessing, multiuser capabilities
        o	Kernel space vs user space
        o	OS boot sequence (generic model)
    •	🧠 Core OS Components
        o	Kernel: role and sub-components
        o	Process Scheduler: algorithms and priorities
        o	Memory Manager: virtual memory, paging
        o	File System Manager
        o	Device Drivers and Hardware Abstraction Layer (HAL)
        o	System Calls and APIs
        o	User Interface: CLI vs GUI
        o	Daemons/Services background processes
        o	Interprocess Communication (IPC) models
        o	Module loading and kernel extensions
    •	🧮 Process Management
        o	What is a process?
        o	States: Ready, Running, Waiting, Terminated
        o	Process Control Block (PCB)
        o	Threads: multithreading, thread pools
        o	Scheduling strategies: FIFO, Round-Robin, Multilevel Queue
        o	Context switching
        o	Foreground vs background processes
        o	Process hierarchy and parent-child relationships
        o	Resource allocation per process
        o	Orphan and zombie processes
    •	🧬 Memory Management
        o	Address spaces: logical vs physical
        o	Paging, segmentation
        o	Page tables and TLBs (Translation Lookaside Buffers)
        o	Virtual memory and swap
        o	Memory fragmentation
        o	Allocation techniques: First Fit, Best Fit, Buddy System
        o	Memory protection and isolation
        o	Demand paging and page faults
        o	Heap vs stack memory regions
        o	Shared memory models
    •	📁 File System Management
        o	File attributes: metadata, permissions, timestamps
        o	File types and extensions
        o	Directory structures: single-level, tree, acyclic graphs
        o	Mounting and partitions
        o	File system journaling
        o	File locks and access controls
        o	Inodes and data blocks (in Linux)
        o	FAT table structure (Windows)
        o	Symbolic and hard links
        o	File compression and encryption
    •	🔌 Input/Output & Device Management
        o	I/O device categories: character vs block
        o	Device drivers and driver stacks
        o	Interrupts and polling mechanisms
        o	Plug-and-play architecture
        o	Buffering and spooling
        o	DMA (Direct Memory Access)
        o	I/O scheduling
        o	USB stack, PCI management
        o	Driver signing and trust chains
        o	Hot-swapping devices
    •	🔒 User & Access Control
        o	Authentication: local, federated, biometric
        o	Authorization: DAC, MAC, RBAC
        o	Session control and isolation
        o	Access tokens and privileges
        o	User roles and permission groups
        o	Credential storage mechanisms
        o	Principle of least privilege
        o	Security identifiers and ACLs
        o	Login types: console, remote, SSH, RDP
        o	User namespaces (Linux container model)
    •	🔁 Multitasking, Multithreading, Multiprocessing
        o	Differences and use-cases
        o	CPU affinity and thread pinning
        o	Thread vs process isolation
        o	Kernel-mode vs user-mode threading
        o	Preemptive vs cooperative multitasking
        o	Symmetric multiprocessing (SMP) and scheduling
        o	Hyper-threading awareness
        o	Locks, semaphores, and race conditions
        o	Thread synchronization issues
        o	Deadlocks and starvation
    •	📡 Networking Basics in OS
        o	OSI layer integration into system stack
        o	NIC drivers and interface configuration
        o	Sockets and port binding
        o	TCP/IP stack and loopback interfaces
        o	Network configuration files
        o	Firewalls and packet filters
        o	Connection management and timeouts
        o	DNS resolver settings
        o	DHCP client configuration
        o	ICMP error handling
    •	🧰 System Configuration & Maintenance
        o	System logs and log rotation
        o	Configuration file hierarchy
        o	Scheduled jobs (cron, task scheduler)
        o	Time sync (NTP, system clock)
        o	Locale and language settings
        o	System updates and patching
        o	Bootloader configuration
        o	Init systems (init, systemd, launchd)
        o	Emergency and recovery modes
        o	Snapshot and rollback mechanisms


🪠 Windows Internals
    •	🔧 Windows Architecture Overview
        o	Kernel mode vs User mode
        o	Executive, HAL, Kernel, Subsystems
        o	Native APIs vs Win32 APIs
        o	Object Manager
        o	Registry subsystem
        o	Environment subsystems (e.g., POSIX, WoW64)
        o	Windows Session and Window Station concepts
    •	🔢 Filesystems and Storage
        o	NTFS vs FAT32 vs exFAT
        o	Alternate Data Streams (ADS)
        o	Cluster sizes, MFT, journaling
        o	Symbolic links and junction points
        o	Encryption (EFS)
        o	Disk Quotas
        o	Volume Shadow Copy Service (VSS)
        o	Diskpart, Mountvol, Disk Management
        o	BitLocker fundamentals
    •	📁 Windows Registry
        o	Registry structure: Hives, Keys, Values
        o	Important hives: HKLM, HKCU, HKCR, HKU, HKCC
        o	Boot time configuration
        o	Autostart locations
        o	Registry permissions and auditing
        o	REG files and automation
        o	Using reg.exe, regedit, PowerShell
        o	Malware persistence in registry
        o	Virtualized registry for UWP and WoW64
    •	🌐 User and Permission Management
        o	User types: local, domain, system
        o	NTLM and Kerberos overview
        o	User Account Control (UAC)
        o	SIDs and RIDs
        o	ACLs, ACEs, DACL, SACL
        o	Effective permissions calculation
        o	Security principals and tokens
        o	Using icacls, whoami, takeown
        o	Integrity levels and AppContainer
    •	⚖️ Services and Scheduled Tasks
        o	Service Control Manager (SCM)
        o	services.msc and sc.exe
        o	Creating and configuring services
        o	Service permissions and SDDL strings
        o	Service start types
        o	Scheduled Tasks via Task Scheduler
        o	Event-based triggers
        o	Task XML configuration files
        o	Persistence and privilege escalation vectors
        o	Monitoring scheduled tasks
    •	🤜 PowerShell Internals
        o	Cmdlets vs functions vs scripts
        o	Execution policies
        o	PowerShell profiles and persistence
        o	Modules and importing
        o	Objects and pipelines
        o	Remoting and Invoke-Command
        o	Logging and transcription
        o	Using PowerShell to manage system settings
        o	Security features (Constrained Language Mode)
        o	PS logging (event IDs, transcripts)
    •	🔄 Process, Thread & Memory Management
        o	Processes, threads, handles, jobs
        o	Process Explorer & Process Monitor tools
        o	DLL injection and reflective DLLs
        o	Memory regions: heap, stack, image
        o	Virtual memory and paging
        o	Working set, commit charge
        o	Handle tables and leaks
        o	Windows Internals tools (VMMap, RAMMap)
        o	Debugging symbols (PDBs)
        o	Crash dump analysis
    •	🌌 Boot Process & Startup
        o	BIOS vs UEFI
        o	Secure Boot
        o	Boot Configuration Data (BCD)
        o	Bootmgr, winload, winresume
        o	Safe mode, recovery environment
        o	Boot logs and troubleshooting
        o	Autostart locations (registry, startup folders)
        o	Startup Repair, MSConfig
    •	🔎 Logging and Event Tracing
        o	Event Viewer overview
        o	Windows event log types
        o	Event log locations (evtx)
        o	Important security and system event IDs
        o	Custom views and filters
        o	Forwarded events
        o	ETW (Event Tracing for Windows)
        o	Sysmon basics
        o	Log archiving and retention
    •	🛡️ Windows Security Features
        o	Windows Defender architecture
        o	SmartScreen
        o	Controlled Folder Access
        o	Credential Guard
        o	Device Guard
        o	Windows Firewall and advanced rules
        o	AppLocker and WDAC
        o	Security baselines
        o	LSA protection
    •  ⌛ Command Line Fundamentals (CMD)
        •	Overview of cmd.exe
        •	Command interpreter vs scripting engine
        •	Internal vs external commands
        •	Command chaining (&&, ||, &)
        •	Command history and navigation
        •	Variables and environment variables
        •	Redirection (>, >>, <) and piping (|)
        •	Wildcards and globbing (*, ?)
        •	Using help and /? syntax
        o	Navigating the filesystem with cd, dir, cls, tree
        o	File operations: copy, move, del, ren, mkdir, rmdir
        o	Viewing system info: systeminfo, tasklist, ipconfig, netstat
        o	Managing processes: taskkill, start, shutdown
        o	Network operations: ping, tracert, net use, net view, arp, nslookup
        o	Scripting basics: .bat files, echo, set, if, for, call, goto
        o	Registry operations: reg add, reg query, reg delete
        o	Permissions and users: net user, net localgroup, runas
        o	File comparison and checksum: fc, comp, certutil -hashfile
        o	Encoding and decoding base64: certutil -encode, certutil -decode
        o	Downloading files: certutil -urlcache -split -f for remote files
        o	Digital certificate utilities: certutil -store, certutil -verify, certutil -dump
        o	Advanced batch scripting examples
        ✍️ File & Folder Operations:
            o	dir, cd, mkdir, rmdir, del, copy, move, xcopy, robocopy
            o	Attributes: attrib, icacls
            o	tree, fsutil
            o	Hidden/system files
            o	Recursive deletion
        ⚙️ System Information & Configuration
            o	systeminfo, hostname, ver, set, setx
            o	tasklist, taskkill
            o	wmic basics
            o	ipconfig, netstat, ping, tracert
            o	net use, net view, net session
            o	assoc, ftype
        ⏱ Scheduling & Automation
            o	Creating batch files (.bat)
            o	Using schtasks to create scheduled tasks
            o	Startup folder scripts
            o	call, goto, pause, choice, if, for, setlocal
            o	Comments and script headers
        🌐 Networking Commands
            o	ping, tracert, pathping
            o	netsh basics
            o	ipconfig /all
            o	arp, nbtstat, route print, netstat -ano
            o	telnet and ftp
            o	DNS lookups with nslookup
        ⚖️ User and Access Management
            o	net user, net localgroup, net group
            o	whoami, runas, echo %username%
            o	cacls, icacls, takeown
            o	Modifying ownership and permissions
        •	🛠️ Troubleshooting and Diagnostics
            o	Reading logs with wevtutil
            o	sfc /scannow, chkdsk, DISM
            o	echo, pause, cls, color
            o	Testing scripts safely
            o	Interacting with .reg files
  •	📁 File Types and Structures
        o	Executable formats: .exe, .dll, .sys, .bat, .ps1
        o	Document formats: .docx, .pdf, .rtf, .txt
        o	Archive formats: .zip, .rar, .7z, .tar.gz
        o	Image formats: .jpg, .png, .bmp, .svg
        o	Multimedia formats: .mp4, .mp3, .avi, .mkv
        o	Configuration formats: .ini, .conf, .yaml, .json, .xml
        o	Log files: structure, delimiters, timestamps, and severity levels
        o	Proprietary vs Open formats
    
  • 🧮 Encoding and Character Sets
        o	ASCII and Extended ASCII
        o	Unicode: UTF-8, UTF-16, UTF-32
        o	Base64 encoding and decoding
        o	URL encoding
        o	Hexadecimal and Binary representations
        o	Endianness (Big-endian vs Little-endian)
        o	BOM (Byte Order Mark) and its impact on file parsing
    •	🧪 Parsing and Manipulation Tools
        o	cat, less, more, head, tail, strings
        o	xxd, hexdump, binwalk, file
        o	jq, xmlstarlet, yq, csvkit
        o	iconv and character encoding conversion
    •	🔎 File Metadata & Attributes
        o	File timestamps: Created, Modified, Accessed
        o	File permissions and ACLs
        o	Alternate Data Streams (ADS) on NTFS
        o	Hidden/system attributes
        o	Signature validation and hash comparison (MD5, SHA1, SHA256)
    •	📦 Forensics Considerations
        o	Understanding file carving
        o	Recognizing anomalies in file headers/footers
        o	Common obfuscation techniques in documents (e.g., macros)
        o	File magic numbers


🐗 Linux Fundamentals
    •	🐧 Linux Operating System Overview
        o	History and evolution of Linux
        o	Linux kernel vs distributions
        o	Open-source philosophy and licensing (GPL)
        o	Use cases: servers, desktops, embedded, IoT
    •	🏗️ Linux Filesystem Structure
        o	Hierarchical directory structure (/ root)
        o	Essential directories:
            o	/etc – system config
            o	/home – user directories
            o	/var – variable files/logs
            o	/usr – user binaries, libraries
            o	/bin, /sbin, /lib, /lib64
            o	/dev, /proc, /sys, /run
        o	Filesystem types: ext4, XFS, Btrfs
        o	Mounting and unmounting
        o	Fstab and persistent mounts
    •	🔄 Boot Process & Runlevels
        o	BIOS/UEFI to GRUB to kernel
        o	Init systems: SysVinit vs systemd
        o	Kernel loading and initrd
        o	Targets (runlevels) in systemd
        o	systemctl, journalctl, dmesg
    •	🧑‍💻 Users, Groups & Permissions
        o	/etc/passwd, /etc/shadow, /etc/group
        o	File permissions (rwx), chmod, chown, umask
        o	SUID, SGID, Sticky Bit
        o	adduser, useradd, usermod, groupadd
        o	User context switching: su, sudo, /etc/sudoers
    •	🗂️ Package Management
        o	Debian-based (apt, dpkg)
        o	Red Hat-based (yum, dnf, rpm)
        o	Arch-based (pacman)
        o	Building from source: ./configure && make && make install
        o	Snap, Flatpak, AppImage
    •	🔎 Process Management
        o	Foreground vs background processes
        o	ps, top, htop, kill, nice, renice
        o	systemctl for managing daemons
        o	Jobs: jobs, fg, bg, disown
        o	Signals and signal handling
    •	🧰 Command Line Proficiency (Bash)
        o	Navigation: cd, ls, pwd
        o	File operations: touch, cp, mv, rm
        o	Viewing: cat, less, more, tail, head
        o	Text manipulation: grep, cut, awk, sed, tr
        o	Redirection: >, >>, <, |, tee
        o	Variables and quoting
        o	Command substitution: $(...), backticks
        o	Globbing and wildcards: *, ?, []
        o	Loops and conditionals in bash
    •	📜 Shell Scripting
        o	Creating scripts (#!/bin/bash)
        o	Arguments: $1, $2, $@, $#
        o	Control flow: if, case, while, for, until
        o	Functions and return values
        o	Exit codes and error handling
        o	Logging and debug (set -x, trap)
    •	🌐 Networking in Linux
        o	ip, ifconfig, ip a, ip route
        o	Hostname and DNS: /etc/hosts, /etc/resolv.conf
        o	Network services: sshd, nginx, netcat
        o	ping, netstat, ss, tcpdump, traceroute, curl
        o	Opening ports and firewalls: ufw, iptables
        o	SSH key management: ssh-keygen, ssh-copy-id, authorized_keys
    •	🧩 System Monitoring & Logs
        o	System logs in /var/log
        o	journalctl for systemd logs
        o	uptime, free, vmstat, iostat
        o	top, htop, iotop, dstat
        o	Custom log management with logrotate
    •	🛡️ Linux Security Fundamentals
        o	Understanding root and least privilege
        o	sudo, visudo, /etc/sudoers.d
        o	AppArmor and SELinux basics
        o	chmod, chown, setfacl
        o	Secure shell (SSH) practices
        o	Disabling unused services


☁️ Cloud Computing Fundamentals
    •	☁️ Introduction to Cloud Computing
        o	Definition of Cloud Computing
        o	History and evolution
        o	Benefits: scalability, elasticity, pay-as-you-go
        o	Cloud service models: IaaS, PaaS, SaaS
        o	Deployment models: Public, Private, Hybrid, Community
    •	🏢 Cloud Service Providers (CSPs)
        o	Overview of major CSPs: AWS, Azure, GCP
        o	Regional architecture and availability zones
        o	Free tiers, pricing calculators, and billing concepts
    •	🧰 Core Cloud Services
        o	Compute: EC2, Azure VM, GCE
        o	Storage: S3, Blob, GCS Buckets
        o	Databases: RDS, Azure SQL, Cloud SQL
        o	Networking: VPC, Subnets, NAT, Load Balancing
        o	IAM: Identity and Access Management across platforms
    •	🔐 Cloud Identity and Security
        o	IAM Users, Groups, Policies
        o	MFA, Key Rotation, Least Privilege
        o	Encryption at rest vs in transit
        o	Cloud-specific firewalls (e.g., Security Groups, NSGs)
        o	Shared Responsibility Model
        •	🖧 Cloud Networking & DNS
        o	VPC setup and segmentation
        o	Public vs private subnets
        o	Route tables, internet gateways, NAT
        o	DNS services: Route53, Cloud DNS, Azure DNS
        o	Load balancers: ELB, ALB, NLB, Application Gateway
    •	🚀 Automation & Infrastructure as Code (IaC)
        o	Overview of IaC concepts
        o	Tools: Terraform, AWS CloudFormation, Azure Bicep
        o	Version control and CI/CD integration
        o	Modularization and DRY principles
    •	🕵️‍♂️ Monitoring, Logging & Alerts
        o	AWS CloudWatch, Azure Monitor, GCP Stackdriver
        o	Metric collection and custom dashboards
        o	Centralized log collection and analysis
        o	Alert rules, thresholds, and notifications
    •	🔄 Cloud Resource Lifecycle
        o	Provisioning, tagging, and naming conventions
        o	Scheduled auto-scaling and shutdowns
        o	Cost optimization techniques
        o	Reserved Instances vs Spot Instances
    •	📦 Cloud Storage Deep Dive
        o	Object storage vs block storage vs file storage
        o	S3 storage classes and lifecycle policies
        o	Storage redundancy and cross-region replication
        o	Blob tiers: hot, cool, archive
    •	🔐 Cloud Compliance and Governance
        o	Identity Federation and SSO
        o	Policy enforcement (SCPs, Azure Policies)
        o	GDPR, HIPAA, ISO, SOC, NIST in cloud
        o	Audit logs and compliance reports


🧠 Programming & Scripting Foundations
    •	🔤 Programming Concepts Overview
        o	What is programming?
        o	Compilation vs interpretation
        o	Static vs dynamic typing
        o	Memory management basics (stack vs heap)
        o	Syntax, semantics, and control flow
    •	💻 C/C++ Foundations
        o	Compilation toolchain (GCC, Clang, MSVC)
        o	Variables and data types (int, float, char, pointers)
        o	Control structures (if, switch, for, while, do-while)
        o	Functions and stack frames
        o	Arrays, strings, pointers and pointer arithmetic
        o	Memory management: malloc, free, calloc, realloc
        o	Structs, unions, enums
        o	Header files and multiple source files
        o	Makefiles and build systems
        o	Debugging with gdb
    •	🔠 C# Fundamentals
        o	CLR and .NET overview
        o	Basic syntax and types
        o	Classes, interfaces, inheritance
        o	Properties, fields, and methods
        o	Events and delegates
        o	Exception handling
        o	LINQ basics
        o	Assemblies and compilation
        o	Windows Forms & Console Applications
    •	🐚 Scripting with Bash
        o	Variables and quoting
        o	Arithmetic and string operations
        o	Conditional expressions ([ ], [[ ]])
        o	Looping structures (for, while, until)
        o	Functions, arguments, and return values
        o	Script parameters: $1, $@, $#
        o	File operations and redirection
        o	Automating common tasks
    •	🐍 Python Fundamentals
        o	Syntax and indentation
        o	Built-in data types (int, list, dict, set)
        o	Flow control (if, for, while)
        o	Functions, modules, and packages
        o	Object-oriented programming in Python
        o	Working with files and directories
        o	Exception handling
        o	Virtual environments and pip
        o	os, sys, subprocess, socket, requests
    •	⚙️ Development Tools & Practices
        o	Version control: Git basics
        o	IDEs and text editors (VS Code, CLion, Vim, etc.)
        o	Command line build tools
        o	Basic unit testing frameworks
        o	Using documentation and manuals
        o	Reading and understanding open-source code
    •	🧪 Practical Challenges
        o	Building a command-line calculator (C)
        o	File parser script (Python/Bash)
        o	Simulating process scheduler (C++)
        o	Simple REST client (C# or Python)
        o	Memory game or number guesser app


📦 Software Development Environments
        •	🧑‍💻 Integrated Development Environments (IDEs)
                o	What is an IDE?
                o	Examples: Visual Studio, VS Code, IntelliJ, Eclipse
                o	Extensions, plugins, linters
                o	Debuggers and breakpoints
                o	Build systems (CMake, MSBuild, Gradle)
        •	🛠️ Compilers & Interpreters
                o	GCC, Clang, MSVC
                o	.NET CLR and Mono
                o	Python and Bash interpreters
                o	Just-in-Time vs Ahead-of-Time compilation
                o	Compilation pipelines and optimization flags
        •	🧪 Testing & Debugging Tools
                o	Unit testing frameworks (NUnit, PyTest, Catch2)
                o	Code coverage tools
                o	Memory analyzers (Valgrind, Dr. Memory)
                o	Debugging tools (GDB, WinDbg, LLDB)
        •	📁 Project Structure & Version Control
                o	Directory structure best practices
                o	Configuration files (.env, .gitignore, requirements.txt)
                o	Git fundamentals: clone, commit, branch, merge
                o	Remote repositories: GitHub, GitLab, Bitbucket
                o	Version control strategies: GitFlow, trunk-based dev
        •	📜 Documentation & Standards
                o	Code documentation: docstrings, XML comments
                o	README files and API documentation
                o	Coding conventions and linters
                o	OpenAPI / Swagger for API docs
        •	🧪 Build & CI/CD Systems
                o	Jenkins, GitHub Actions, GitLab CI
                o	Build pipelines: stages and artifacts
                o	Docker integration in CI/CD
                o	Unit and integration test automation
        •	📦 Package Managers
                o	C++: Conan, vcpkg
                o	.NET: NuGet
                o	Python: pip, poetry
                o	Node.js: npm, yarn
                o	Dependency versioning, pinning
        •	🖥️ Cross-Platform Considerations
                o	Windows vs Linux pathing, line endings, permissions
                o	Portable code strategies
                o	Preprocessor macros
        •	🔍 Code Quality & Analysis
                o	Static analysis tools (SonarQube, ESLint, Pylint)
                o	Code smells and anti-patterns
                o	Technical debt management
        •	📄 Software Licensing & Ethics
                o	GPL, MIT, Apache, BSD licenses
                o	Proprietary vs open-source implications
                o	Ethical coding practices and attribution


🧮 Networking
        •	🌐 Networking Fundamentals
                o	What is a Network?
                o	Network Types: LAN, WAN, MAN, PAN
                o	Packet Switching vs Circuit Switching
                o	Network Topologies
                        o	Historical topologies: Token Ring, Bus
                        o	Modern topologies: Star, Mesh, Tree, Hybrid
                o	Network Models
                        o	OSI Model
                        o	TCP/IP Stack
                o	Network Performance Metrics
                        o	Latency, Jitter, Bandwidth, Throughput
                        o	MTU, MSS
                o	Broadcast Domain vs Collision Domain
                        o	Definitions, diagrams, and simulations
                        o	Switch segmentation and VLAN boundaries
                        o	Real-world implications in network design
                o	Message Types: Unicast, Broadcast, Multicast
                        o	Layer 2: MAC unicast, multicast (01:00:5E), broadcast (FF:FF:FF:FF:FF:FF)
                        o	Layer 3: IP unicast, broadcast (255.255.255.255), multicast (224.0.0.0/4)
                        o	IGMP and multicast group management
                        o	ARP and DHCP as broadcast examples
                        o	DNS as unicast example
                        o	Practical packet captures using Wireshark
    •	🧱 Networking Devices (Extended)
                o	Routers
                        o	Static vs dynamic routing
                        o	Default routes
                        o	CIDR and summarization
                o	Switches
                        o	Spanning Tree Protocol (STP, RSTP, MSTP)
                        o	MAC learning and port forwarding decisions
                        o	VLAN trunking (802.1Q)
                        o	Switchport security features
                o	Hubs vs Switches
                        o	Historical role of hubs
                        o	Why switches replaced hubs
                        o	Collision domains in hub networks
                        o	Packet flooding vs MAC-based forwarding
                        o	Demo lab: Sniffing on a hub vs switch
                o	NICs and Interfaces
                        o	Promiscuous mode
                        o	Duplex mismatch issues
                        o	Auto-negotiation
                o	Firewalls
                        o	Deep Packet Inspection (DPI)
                        o	Zone-based firewall logic
                        o	Common vendor CLI: Cisco ASA, Palo Alto
                o	Load Balancers
                        o	Algorithms: Round-robin, least connections
                        o	Health checks
                        o	Application awareness (SSL termination)
                o	Wireless Infrastructure
                        o	SSIDs, channels, encryption (WEP, WPA2, WPA3)
                        o	2.4 GHz vs 5 GHz vs 6 GHz bands
                        o	Access Point roles (controller-based, standalone)
                o	Modems and Gateways
                        o	DSL, Cable, Fiber modems
                        o	NAT behavior in gateways
                        o	Dual NAT and CGNAT explained
    •	🏗️ OSI Model Layers (Expanded)
                o	Physical Layer
                        o	Cable standards: Cat5e, Cat6, Cat6a, Cat7
                        o	Fiber optic types: single-mode, multi-mode
                        o	Signal degradation and attenuation
                        o	Bit-level transmission simulation
                o	Data Link Layer
                        o	Ethernet frame breakdown: Preamble, SFD, MACs, Type, FCS
                        o	Switch loop protection (STP, BPDU Guard)
                        o	VLAN tagging and double tagging (Q-in-Q)
                        o	MAC flooding attacks (brief intro)
                o	Network Layer
                        o	IPv4 fragmentation and reassembly
                        o	Subnetting techniques and exercises
                        o	Route redistribution concepts
                        o	NAT types (static, dynamic, PAT)
                        o	Layer 3 ACLs and firewalling
                o	Transport Layer
                        o	TCP handshake deep dive (SYN, SYN-ACK, ACK)
                        o	Retransmission and sliding window mechanics
                        o	UDP with practical examples: TFTP, SNMP
                        o	Port scans: SYN, FIN, NULL, Xmas (not exploitative yet)
                o	Session Layer
                        o	SSL/TLS handshake overview
                        o	RDP, SMB session creation
                o	Presentation Layer
                        o	Data transformation: ASCII vs Unicode
                        o	SSL/TLS encryption examples
                o	Application Layer
                        o	HTTP headers: Host, Cookie, User-Agent
                        o	DNS record types: A, AAAA, CNAME, MX, TXT
                        o	DHCP options and packet flow (DORA)
                        o	FTP active vs passive mode
                        o	SMTP, IMAP, POP3 comparison


🔐 Security Basics
        •	🛡️ Foundations of Security
                o	What is Information Security?
                        o	Confidentiality, Integrity, Availability (CIA Triad)
                        o	Non-repudiation and Authentication
                        o	Real-world examples of CIA violations
                o	Security Terminology
                        o	Asset, Threat, Vulnerability, Exploit, Risk, Control
                        o	Threat actor types: script kiddies, insiders, nation-states, APTs
                o	Security Principles
                        o	Least privilege
                        o	Defense in depth
                        o	Fail-safe defaults
                        o	Separation of duties
                        o	Security through obscurity (debate)
                o	Types of Controls
                        o	Physical, Administrative, Technical
                        o	Preventive, Detective, Corrective, Deterrent, Recovery
                o	Security Domains
                        o	Physical security
                        o	Network security
                        o	Application security
                        o	Endpoint security
                        o	Data security
                        o	Identity and access management
                        o	Cloud security (relation to cloud foundations)
        •	🔍 Vulnerabilities & Exposure
                o	Common vulnerabilities
                        o	Misconfigurations
                        o	Unpatched systems
                        o	Weak credentials
                        o	Insecure defaults
                        o	Lack of encryption
                o	Public databases
                        o	CVE, CVSS scoring
                        o	NVD, Exploit DB (overview only)
                o	Security misconfigurations examples
                        o	Directory listing
                        o	Default credentials
                        o	Unrestricted ports/services
                o	Software and firmware lifecycle issues
                        o	EOL/legacy systems
                        o	Supply chain vulnerabilities
        •	🔐 Authentication & Authorization Basics
                o	Authentication types
                        o	Single-factor, Two-factor, MFA
                        o	Something you know/have/are
                        o	Passwords, OTPs, Smart cards, Biometrics
                o	Credential Storage Principles
                        o	Hashing vs Encryption
                        o	Salted hashes (bcrypt, scrypt)
                        o	Insecure storage examples (plain text, reversible encryption)
                o	Authorization Models
                        o	RBAC, ABAC, DAC, MAC
                        o	Access Control Lists (ACLs)
                        o	Principle of least privilege
                        o	Segregation of duties
        •	🔒 Encryption Fundamentals
                o	Symmetric vs Asymmetric Encryption
                o	Common algorithms: AES, RSA, ECC
                o	Hashing algorithms: SHA family, MD5 (deprecated)
                o	Encoding vs Encryption vs Hashing
                o	SSL/TLS basics (how HTTPS works)
                o	Certificates and PKI
                        o	Root, intermediate, leaf certs
                        o	Certificate validation and revocation (CRL/OCSP)
        •	📊 Security Policies & Compliance
                o	What are security policies?
                        o	Acceptable Use Policy
                        o	Password Policy
                        o	Data Retention Policy
                        o	Remote Work Policy
                o	Introduction to compliance
                        o	ISO 27001
                        o	NIST 800-series
                        o	SOC 2
                        o	GDPR overview (personal data, consent, DSRs)
                        o	HIPAA overview
        •	🛠️ Security Tools 
                o	Antivirus/Antimalware basics
                o	Host-based firewall (Windows Defender Firewall)
                o	File integrity monitoring
                o	Basic packet filtering firewalls
                o	Centralized log review
        •	🧠 Mindset & Awareness
                o	Security as a continuous process
                o	Red team / blue team concepts 
                o	Security awareness for users
                        o	Phishing recognition
                        o	Social engineering prevention
                        o	Data classification and handling


📁 Filesystems & Storage
        •	💾 Filesystem Concepts
                o	What is a filesystem?
                        o	Purpose and role in OS
                        o	Relation to physical storage
                o	Structure of a filesystem
                        o	Blocks, clusters, sectors
                        o	Inodes (Unix/Linux)
                        o	MFT (Windows NTFS)
                o	File types and metadata
                        o	Regular files, directories, symbolic links
                        o	Permissions and timestamps
                        o	Hidden/system attributes
        •	🧷 Common Filesystems
                o	FAT32
                        o	Legacy use cases
                        o	Max file/partition size
                        o	Lack of permissions
                o	NTFS
                        o	Journaling
                        o	ACL-based permissions
                        o	Alternate data streams (ADS)
                        o	Encryption (EFS)
                o	exFAT
                        o	Use in USB and SD cards
                        o	Compatibility
                o	ext2/ext3/ext4
                        o	Differences in journaling
                        o	Use of inodes
                        o	Linux compatibility
                o	Btrfs, XFS, ZFS (overview)
        •	🧩 Storage Technologies
                o	HDD vs SSD
                        o	Mechanical vs flash memory
                        o	Lifespan, wear leveling
                o	Hybrid drives (SSHD)
                o	NVMe & SATA interfaces
                o	Storage controllers (RAID overview)
                        o	RAID levels: 0, 1, 5, 6, 10
                        o	Software vs Hardware RAID
        •	🗂️ Mounting & Partitioning
                o	Partition tables
                        o	MBR vs GPT
                        o	Primary vs extended partitions
                o	Mounting concepts
                        o	Mount points
                        o	Fstab (Linux)
                        o	Disk Management (Windows)
                o	Formatting and initialization
                        o	Quick format vs full format
                        o	Filesystem check (chkdsk, fsck)
        •	🧪 Practical Tools & Utilities
                o	Windows
                        o	Disk Management GUI
                        o	diskpart, format, chkdsk, fsutil
                        o	BitLocker (intro only)
                o	Linux
                        o	lsblk, fdisk, parted, mkfs, mount, umount
                        o	df, du, fsck, tune2fs, blkid
        •	🔐 Security & Forensics Aspects
                o	Deleted file recovery
                        o	File carving basics
                o	Journaling and write logs
                        o	Use in incident investigation
                o	Hidden data and steganography
                o	Access control implications
                        o	Permissions on file-level
                        o	Filesystem encryption


🧩 Virtualization & Containers
        •	🧰 Virtualization Basics
                o	What is virtualization?
                        o	Concept of abstraction
                        o	Benefits: isolation, scalability, testing environments
                o	Hypervisors
                        o	Type 1 (bare-metal) vs Type 2 (hosted)
                        o	Examples: VMware ESXi, Microsoft Hyper-V, VirtualBox
                o	Guest OS vs Host OS
        •	🖥️ Working with Virtual Machines
                o	Creating VMs
                        o	ISO selection and installation
                        o	Assigning virtual hardware: CPU, RAM, disk, network
                o	Snapshots and cloning
                        o	Use cases for testing and recovery
                o	VM networking modes
                        o	NAT, bridged, host-only
        •	🧱 Containers Fundamentals
                o	What are containers?
                        o	Difference from VMs
                        o	Use of shared OS kernel
                o	Container engines
                        o	Docker: image, container, volume, network
                        o	Podman (rootless alternative)
                o	Dockerfile basics
                        o	Image layering, build process
                o	Docker Compose overview
        •	🕸️ Container Networking
                o	Bridge networks
                o	Host networking
                o	Overlay networks (for clustering)
                o	Port publishing and NAT
        •	🔐 Security Considerations
                o	VM escape basics (concept only)
                o	Container isolation risks
                o	Namespaces and control groups (cgroups)
                o	Image scanning and hardening
        •	🧪 Tools & Utilities
                o	Virtualization
                        o	VirtualBox, VMware Workstation
                        o	QEMU, KVM
                o	Containers
                        o	Docker CLI
                        o	Docker Desktop GUI
                        o	docker inspect, docker exec, docker logs


🔗 Active Directory & Domain Services
        •	🏛️ Core Concepts of Active Directory (AD)
                o	What is AD and why it's used
                o	Centralized authentication and authorization
                o	Domains, trees, forests
                o	Logical & physical structure: DCs, OUs, Sites, Global Catalog
        •	👥 Users, Groups & Access Management
                o	Local vs domain accounts
                o	Group types & scopes
                o	OU design and best practices
                o	Group nesting, RBAC, administrative tiers
                o	GPO basics and deep dive
        •	🧠 Authentication & Trust Models
                o	Kerberos authentication flow (AS, TGS, TGT, ST)
                o	NTLMv1 vs NTLMv2
                o	NTLM authentication flow
                o	Trust relationships
                o	SSO and token delegation
                o	SID, RID, and token structure
                o	Pass-the-Hash (concept only, not exploitation)
        •	🧰 Administrative Tools & Management
                o	Active Directory Users & Computers (ADUC): creating, modifying, disabling accounts
                o	ADAC, GPMC, ADSI Edit
                o	PowerShell Modules for AD
                        o	Creating bulk users and groups
                        o	Enforcing password policies
                        o	Querying trust relationships
                        o	Searching nested groups
        •	🔐 Permissions, ACLs & Delegation
                o	NTFS permissions vs share permissions
                o	Effective permissions
                o	DACL, SACL, ACE entries
                o	Inheritance & blocking
                o	Delegation Wizard use cases
                o	Auditing: enabling and interpreting
        •	📡 DNS Integration & SRV Records
                o	Role of DNS in domain joining
                o	SRV records for Kerberos, LDAP
                o	Dynamic DNS registration
                o	Testing DNS with nslookup, nltest
        •	🧪 Diagnostics & Troubleshooting
                o	Common tools: dcdiag, repadmin, nltest, netdom, whoami
                o	Troubleshooting logon failures
                o	Diagnosing replication issues
                o	Reading AD event logs
        •	🧬 Schema, FSMO Roles & Replication
                o	AD Schema explained
                o	Schema extensions and risks
                o	5 FSMO roles and their responsibilities
                o	Replication flow, latency, and conflict resolution
                o	Site links and replication topology
        •	🧩 Enterprise Design Patterns & Scenarios
                o	Tier 0/1/2 models
                o	Domain isolation vs resource forest
                o	Multi-domain architecture
                o	Trust design in mergers & hybrid clouds
                o	Integration with Azure AD


📚 Fundamental IT Protocols
        •	🌐 Protocol Layers Overview
                o	OSI vs TCP/IP models
                o	Layered approach and encapsulation
        •	💬 Application Layer Protocols (OSI Layer 7)
                o	HTTP/HTTPS: headers, status codes, methods
                o	DNS: record types, resolution flow, recursive vs iterative
                o	SMTP/IMAP/POP3: mail transfer, authentication
                o	DHCP: DORA process, scopes, leases
                o	SNMP: OIDs, community strings, MIB
                o	FTP/SFTP/FTPS: modes, ports, secure transfer differences
                o	LDAP: directory structure, queries, authentication
                o	RDP: security layers, ports, tunneling
                o	SSH: key exchange, secure remote access, port forwarding
                o	SMB: file sharing, NTLM authentication, vulnerabilities
                o	NFS: Unix file sharing basics, mount types
                o	Telnet: insecure terminal access, legacy use cases
        •	📶 Transport Layer Protocols (OSI Layer 4)
                o	TCP: handshake, sequence numbers, retransmissions
                o	UDP: stateless communication, DNS, VoIP
                o	Common ports and services
                o	NAT traversal techniques
        •	🧱 Network Layer Protocols (OSI Layer 3)
                o	IPv4: subnetting, CIDR, classes, ARP
                o	IPv6: addressing, scopes, transition strategies
                o	ICMP: ping, traceroute, types
                o	Routing basics: static vs dynamic, protocols (OSPF, BGP, RIP)
        •	🔌 Data Link Layer Protocols (OSI Layer 2)
                o	Ethernet: MAC addressing, frame format
                o	VLANs and trunking
                o	ARP table and spoofing
                o	STP and loop prevention
        •	⚙️ Physical Layer & Encodings (OSI Layer 1)
                o	Bit transmission, cables, modulation
                o	Signal interference and attenuation
                o	Standards: Cat5/6/7, fiber optics
        •	🔍 Protocol Analysis Tools
                o	Wireshark: filters, decoding protocols
                o	tcpdump, tshark
                o	Netcat, Telnet
                o	nslookup, dig
        •	🧪 Common Network Protocol Attacks (Conceptual)
                o	DNS poisoning (not exploitation)
                o	IP spoofing theory
                o	ARP cache poisoning overview
                o	TCP session hijacking concept
                o	SMB relay attack theory
                o	SSH brute-force risk concept
        •	📘 RFCs & Protocol Documentation
                o	Understanding how to read an RFC
                o	Using protocol standards for troubleshooting


💾 System Administration & IT Operations
        •	🖥️ Workstation Management
                o	Installing and configuring operating systems
                o	Imaging and deployment techniques
                o	Device drivers: understanding, updating, rollback
                o	Windows Update, WSUS
                o	Scheduled Tasks, Task Scheduler management
                o	Time synchronization (NTP)
                o	BIOS vs UEFI configuration
        •	🧰 System Tools and Utilities
                o	Control Panel vs Settings
                o	System Information (msinfo32, dxdiag)
                o	Event Viewer: log types, filtering, diagnosis
                o	Resource Monitor, Performance Monitor
                o	Services (services.msc), service dependencies
                o	MSC snap-ins and their functions
        •	🧼 System Maintenance
                o	Disk Cleanup, Defragmentation
                o	Windows Resource Protection (sfc, DISM)
                o	System Restore and Shadow Copies
                o	Registry backup and restore
        •	🔄 User and Session Management
                o	Local users and groups
                o	Profiles (local vs roaming)
                o	UAC and elevation
                o	Fast user switching and session concurrency
                o	Logon types and authentication flow
        •	🔌 Device and Peripheral Management
                o	Printers and print queues
                o	USB policies and restrictions
                o	Mounting drives, drive letters, network drives
        •	🗃️ Software Management
                o	Installation types: MSI, EXE, Windows Store
                o	Silent installs, deployment automation
                o	Uninstall tools, leftover cleanup
        •	💼 Task Automation & Scripting
                o	PowerShell: cmdlets, pipelines, remoting
                o	CMD: batch scripting, control flow, for loops
                o	Scheduled scripts and task triggers
                o	Automation use cases (shutdowns, backups, logs)
        •	🌐 Remote Access & Support
                o	RDP, VNC, and third-party tools
                o	Windows Remote Assistance
                o	Remote MMC usage, WMI and PowerShell remoting
        •	🔐 Security Configurations
                o	BitLocker configuration and recovery
                o	Group Policy Editor (gpedit.msc) usage
                o	Local Security Policy and auditing
                o	AppLocker, SRP (Software Restriction Policies)
        •	🧭 System Navigation & Accessibility
                o	Environment variables
                o	File Explorer: hidden/system files, view options
                o	Accessibility 


🧪 Software & Application Behavior
        •	📁 How Software Works
                o	What is software: binary vs interpreted
                o	Runtime environments and dependencies
                o	Compilation vs interpretation
                o	Software architecture: monolithic vs microservices
                o	How operating systems load and execute programs
                o	DLLs and shared libraries
                o	Process lifecycle: creation, execution, termination
                o	Threads vs processes
                o	Software update mechanisms
                o	Software packaging and installers (e.g., MSI, EXE, Deb, RPM)
        •	🔍 Application Behavior Analysis
                o	Understanding behavior vs code
                o	Static vs dynamic analysis
                o	Resource usage (RAM, CPU, Disk, Network)
                o	Memory allocation patterns
                o	File system interactions
                o	Registry interactions (Windows)
                o	Network connections and outbound calls
                o	Common logging behaviors
                o	Interprocess communication (IPC)
                o	Crash and exception handling
        •	🧪 Testing & Instrumentation
                o	Using Sysinternals Suite (ProcMon, ProcExp, TCPView)
                o	Dependency Walker, PE Studio
                o	Monitoring file and registry access
                o	Tracking process trees and child processes
                o	Debuggers overview (x64dbg, WinDbg, GDB)
                o	API call tracing and hooking
                o	Environment sandboxing and behavior isolation
                o	Event Viewer and Application Logs
        •	🧰 Configuration & Tuning
                o	Software configuration files and flags
                o	Feature toggles
                o	Licensing mechanisms
                o	Telemetry and analytics opt-out
                o	Startup behaviors and autostart mechanisms
                o	Handling corrupted config states
        •	🏗 Examples of Software Types
                o	System-level tools (e.g., drivers, services)
                o	User-facing applications (e.g., browsers, mail clients)
                o	Background services and daemons
                o	CLI tools vs GUI software
                o	Web-based apps (client-server model)
                o	Mobile apps (Android/iOS architecture)


CYBER

🛡️ Security Appliances & Defensive Mechanisms
        •	🔥 Firewalls (FW)
                o	Types of firewalls:
                        o	Packet-filtering
                        o	Stateful inspection
                        o	Proxy-based (Application Layer)
                        o	Next-Generation Firewall (NGFW)
                o	Inbound vs outbound filtering
                o	Rules and policies (allow/deny, ports, protocols)
                o	Zone-based firewalling and segmentation
                o	Logging and alerting
                o	Integration with SIEM and IPS/IDS
        •	🛑 Network Access Control (NAC)
                o	Purpose: Restrict access based on identity, posture, or location
                o	802.1X authentication and RADIUS
                o	Posture assessment: AV installed, patch level, domain join
                o	Quarantine VLANs and remediation portals
                o	Agent-based vs agentless NAC solutions
                o	Integration with AD, MDM, and threat intelligence
        •	🌀 Load Balancers (LB)
                o	Types:
                        o	L4 (Transport Layer) load balancing
                        o	L7 (Application Layer) load balancing
                o	Session persistence (sticky sessions)
                o	SSL termination vs SSL passthrough
                o	Health checks and failover
                o	Load balancing algorithms:
                        o	Round robin
                        o	Least connections
                        o	IP hash
                o	Reverse proxy integration
        •	🛡️ Web Application Firewalls (WAF)
                o	Function: Filter HTTP(S) traffic to/from web apps
                o	Signature-based vs behavioral WAF
                o	OWASP Top 10 protections
                o	Protection against:
                        o	SQL Injection
                        o	XSS
                        o	CSRF
                        o	File inclusion
                        o	Command injection
                o	Positive vs negative security models
                o	Deployment modes:
                        o	Reverse proxy
                        o	Transparent bridge
                        o	Inline/Out-of-band
        o	Cloud-based WAF vs on-prem (e.g., AWS WAF, Cloudflare)
        •	🧠 Intrusion Detection/Prevention Systems (IDS/IPS)
        o	Signature-based vs anomaly-based detection
        o	Network-based (NIDS) vs host-based (HIDS)
        o	Inline (IPS) vs passive (IDS)
        o	Integration with firewall, SIEM, and EDR/XDR
        o	Common tools: Snort, Suricata, Zeek (Bro)
        •	🔍 Endpoint Detection & Response (EDR/XDR)
                o	Purpose: Monitor, detect, and respond to endpoint threats
                o	Features:
                        o	Real-time telemetry
                        o	Behavior-based detection
                        o	Threat hunting and forensics
                        o	Automated response actions
                o	Examples: CrowdStrike, SentinelOne, Microsoft Defender ATP
        •	🔄 Security Information and Event Management (SIEM)
                o	Central logging and event correlation
                o	Rule-based alerting and dashboards
                o	Integrations with FW, IDS/IPS, NAC, WAF, etc.
                o	Log retention and compliance (e.g., PCI-DSS, ISO 27001)
                o	Threat intelligence feeds and enrichment
                o	Examples: Splunk, QRadar, ELK Stack, Azure Sentinel
        •	🧰 DLP (Data Loss Prevention)
                o	Monitoring and controlling sensitive data flows
                o	Channels: Email, web, USB, clipboard
                o	Detection methods:
                        o	Keyword matching
                        o	Regex
                        o	Fingerprinting
                        o	Machine learning-based classification
                o	Integration with mail servers, proxies, and endpoints
        •	📡 Email Security Gateways (SEG)
                o	Spam filtering, malware scanning, and phishing protection
                o	DKIM, SPF, DMARC enforcement
                o	Sandboxing suspicious attachments
                o	URL rewriting and time-of-click protection
        •	🔐 Encryption Gateways / VPN Concentrators
                o	Secure tunneling for remote access (IPSec, SSL-VPN)
                o	Site-to-site VPN and remote client VPN
                o	Authentication mechanisms: Certificates, 2FA, LDAP
                o	Integration with NAC and SIEM
        •	⚙️ Network Packet Brokers (NPB)
                o	Aggregating and filtering network traffic for monitoring
                o	Load balancing data to multiple tools
                o	Packet slicing, masking, and timestamping
        •	📦 Deliverables & Insights
                o	Topology map of security appliance placement
                o	Policies and configurations review
                o	Effectiveness analysis per control (e.g., blocked threats, alert volume)
                o	Gap analysis and architecture improvement suggestions
                o	Compliance mapping (e.g., ISO, NIST, PCI)
                o	Recommendations for tuning, upgrades, or redundancy


🔒 Cybersecurity Foundations
        •	🌐 Cybersecurity Principles & Domains
                o	CIA Triad (Confidentiality, Integrity, Availability)
                o	Risk vs Threat vs Vulnerability
                o	Security controls: Preventive, Detective, Corrective
                o	Threat modeling: STRIDE, DREAD
                o	Attack surface & threat vectors
                o	Kill chains & attack lifecycles
                o	Common attacker motivations (crime, espionage, hacktivism, etc.)
                o	Ethics, legality, and responsible disclosure
        •	🧠 Mindsets & Disciplines
                o	Red Team vs Blue Team vs Purple Team
                o	Adversarial thinking
                o	Offense vs Defense perspectives
                o	Attacker vs defender tooling asymmetry
                •	🏛 Cybersecurity Ecosystem
                o	Cybersecurity roles and career paths
                o	Standards: ISO 27001, NIST, MITRE ATT&CK
                o	Laws & regulations: GDPR, HIPAA, CCPA, Privacy Protection Law 
                o	Certification landscape: OSCP, CISSP, CISM, CEH, etc.
        •	🔐 Authentication & Authorization
                o	Identity, accounts, credentials, tokens
                o	Authentication types: knowledge, possession, inherence
                o	MFA, SSO, OAuth2, OpenID Connect
                o	Role-Based Access Control (RBAC), ABAC
        •	💥 Common Attacks (General)
                o	Phishing, smishing, vishing
                o	Brute force and credential stuffing
                o	Social engineering
                o	Man-in-the-middle
                o	Replay attacks
                o	Malware categories (worms, trojans, ransomware, spyware)


📰 OSINT (Open Source Intelligence)
        •	🕵️‍♂️ Introduction to OSINT
                o	Definition and value of OSINT in cybersecurity
                o	Legal and ethical boundaries
                o	Difference between passive and active information gathering
                o	Role in reconnaissance and threat intelligence
        •	🌎 Data Sources and Surface Levels
                o	Surface Web: blogs, company websites, public records
                o	Deep Web: subscription-only resources, academic databases
                o	Dark Web: Tor-accessible markets, leak sites, forums
                o	Paste sites (Pastebin, Ghostbin), file sharing platforms
                o	Code repositories (GitHub, GitLab, Bitbucket)
                o	Social media platforms: Facebook, LinkedIn, Twitter, TikTok
                o	Domain registries, WHOIS, DNS records, MX records
                o	Search engines beyond Google: Yandex, Bing, DuckDuckGo
        •	⚖️ OSINT Techniques & Methodologies
                o	Google dorking (intitle, inurl, filetype, etc.)
                o	Metadata analysis in images/docs (EXIF, FOCA)
                o	Subdomain enumeration
                o	DNS zone transfers and passive DNS analysis
                o	Email harvesting, breach lookup (haveibeenpwned, dehashed)
                o	Company structure & employee enumeration (LinkedIn, Hunter.io)
                o	Git repo leaks and exposed credentials
                o	Pastebin & Telegram leak tracking
                o	Threat actor tracking via aliases, PGP keys, reused nicknames
        •	🔧 OSINT Tools
                o	Recon-ng, theHarvester, SpiderFoot, Maltego
                o	FOCA, Shodan, Censys, ZoomEye, BinaryEdge
                o	GitRob, truffleHog, GitLeaks
                o	MetaGoofil, exiftool, pdf-parser.py
                o	Google Hacking Database (GHDB)
                o	Social-analyzer, Creepy, Sherlock
        •	🌐 Infrastructure Enumeration
                o	IP address mapping, ASN and BGP lookups
                o	SSL certificate transparency (crt.sh, censys.io)
                o	Cloud asset exposure (S3 buckets, Azure blobs)
                o	IoT search engines (Shodan filters, Censys banners)
        •	💼 Use Cases of OSINT
                o	Pre-engagement reconnaissance in pentests
                o	Threat intelligence enrichment
                o	Brand monitoring and executive protection
                o	Attack surface mapping
                o	Insider threat detection
                o	Phishing infrastructure tracking
                o	Vulnerability disclosure & responsible reporting
        •	✉️ Operational Security (OPSEC)
                o	Protecting analyst identity (VPN, Tor, burner accounts)
                o	Avoiding search engine fingerprinting
                o	Decoy traffic and anonymized browsing
        •	📝 Reporting OSINT Findings
                o	Structuring OSINT results: who, what, when, how
                o	Correlating findings to targets (companies or individuals)
                o	Annotating timelines and relationships
                o	Visualizing intel with graphs (Maltego, SpiderFoot, custom tooling)
                o	Redacting sensitive or unnecessary personal data


🔍 Penetration Testing 
        •	🧭 Pentest Lifecycle
                o	Understanding scope, impact, and goals
                o	Preparing an effective Rules of Engagement (ROE)
                o	Gathering legal authorization (get out of jail letter)
                o	Choosing methodology: PTES, OWASP, NIST SP800-115, custom hybrid
                o	Environment type: corporate, cloud, hybrid, ICS, IoT
                o	Reporting expectations, standards, and deliverables
        •	🛠 Reconnaissance & OSINT
                o	Passive Recon:
                        o	WHOIS lookups and domain metadata
                        o   Shodan
                        o	DNS enumeration (AXFR, zone transfers, subdomain brute-force)
                        o	Google dorking and advanced search operators
                        o	Metadata extraction from files (e.g. exiftool, PDFid)
                        o	Social media profiling, LinkedIn scraping, name generation tools
                        o	Certificate transparency search (crt.sh, censys.io)
                o	Active Recon:
                        o	Ping sweeps, traceroute, TTL analysis
                        o	Port scanning (Nmap, Masscan, Unicornscan)
                        o	Service detection and versioning (banner grabbing, Nmap scripts)
                        o	Network topology fingerprinting
                o	Tool Arsenal:
                        o	theHarvester, SpiderFoot, Maltego, Amass, FOCA, DNSdumpster
                        o	GitHub & GitLab dorking tools, Shodan, BinaryEdge
        •	🌐 Scanning & Enumeration
                o	Host discovery and network segmentation mapping
                o	Service enumeration:
                        o	SMB (Enum4linux, smbclient, CrackMapExec, rpcclient)
                        o	SNMP (snmpwalk, onesixtyone)
                        o	LDAP, RDP, FTP, HTTP, DNS, SIP, SMTP, etc.
                o	Web Enumeration:
                        o	Hidden files/folders (dirsearch, gobuster, ffuf)
                        o	Fingerprinting (whatweb, builtwith, wafw00f)
                        o	Favicon hash matching, JS file analysis, robots.txt
                o	Vulnerability Scanning:
                        o	Nessus, OpenVAS, Qualys, Nexpose
                        o	Nikto, Nuclei, Burp Suite active/passive scans
        •	🔓 Exploitation Techniques
                o	Credential attacks:
                        o	Bruteforce (Hydra, Medusa, Patator)
                        o	Password spraying, hash cracking (John, Hashcat)
                        o	Kerberoasting, AS-REP Roasting, Pass-the-Hash
                o	Web exploitation:
                        o	Injection types (SQLi, XSS, XML, command, LDAP, SSTI)
                        o	SSRF, CSRF, IDOR, Open Redirect, HTTP Smuggling
                        o	File inclusion and upload abuses (LFI, RFI)
                        o	CORS misconfiguration, JWT manipulation, path traversal
                o	CMS vulnerabilities:
                        o	WordPress, Joomla, Drupal modules/themes/plugins
                        o	Exploitation via WPScan, droopescan, wpscan + metasploit
                o	Binary exploitation (basics):
                        o	Buffer overflow, ROP chains, shellcode injection
                        o	SEH overwrite, egghunting, exploit dev frameworks
                o	Toolkits:
                        o	Metasploit, Empire, Covenant, Cobalt Strike (demo only)
                        o	Custom payloads with msfvenom, Veil-Evasion, Donut
                        o	Antivirus evasion basics (obfuscation, packing, crypters)
        •	📦 Post-Exploitation
                o	Local enumeration:
                        o	OS info, processes, services, startup tasks
                        o	Installed software, environment variables
                        o	Scheduled tasks, WMI events, registry autoruns
                o	Privilege Escalation:
                        o	Windows: AlwaysInstallElevated, unquoted paths, DLL hijacking
                        o	Linux: sudo misconfigs, SUID binaries, PATH manipulation
                        o	Tools: winPEAS, LinPEAS, BeRoot, PowerUp, GTFObins
                o	Credential harvesting:
                        o	Dumping LSASS (Mimikatz, procdump, nanodump)
                        o	secretsdump.py, LaZagne, browser credential storage
                o	Lateral Movement:
                        o	RDP, PSExec, WMI, DCOM, SMB shares, Token impersonation
                        o	Domain escalation via DCsync, DCSHADOW, delegation abuse
                o	Persistence:
                        o	Scheduled tasks, startup folders, registry, WMI, services
                        o	Golden Ticket, Silver Ticket, skeleton key techniques
                o	Data exfiltration, evasion, and cleanup:
                        o	Encoding, staging, chunking (DNS, HTTP, FTP)
                        o	Anti-forensics: timestomping, log wiping, clearing prefetch
        •	📃 Reporting & Deliverables
                o	Executive summaries tailored to business/management
                o	Technical details with reproduction steps
                o	Proof-of-Concepts (PoCs) with screenshots
                o	Risk ratings (CVSSv3, business impact assessment)
                o	Remediation advice: short-term vs long-term
                o	Mapping to frameworks: MITRE ATT&CK, OWASP Top 10
                o	Optional appendices: tool outputs, full logs, hashes
                o	Communication strategies: email, in-person briefings, PDF/interactive reports

        •  🕸 OWASP Top 10 & Web Application Security
                •	Overview of OWASP organization and community projects
                •	OWASP Testing Guide v4 methodology
                •	OWASP Top 10 (latest version)
                        o	A01: Broken Access Control
                        o	A02: Cryptographic Failures
                        o	A03: Injection
                        o	A04: Insecure Design
                        o	A05: Security Misconfiguration
                        o	A06: Vulnerable and Outdated Components
                        o	A07: Identification and Authentication Failures
                        o	A08: Software and Data Integrity Failures
                        o	A09: Security Logging and Monitoring Failures
                        o	A10: Server-Side Request Forgery (SSRF)
                •	Manual testing vs automated testing
                •	Testing tools:
                        o	Burp Suite Professional (manual + extensions)
                        o	ZAP Proxy
                        o	Nikto, dirsearch, ffuf, nuclei
                        o	Browser developer tools and proxying
                •	Exploitation techniques per category
                •	Real-world case studies (e.g., Capital One SSRF, Equifax SQLi)
                •	Secure coding countermeasures for each OWASP Top 10 category
                •	Mapping to CWE IDs, MITRE ATT&CK techniques, and compliance requirements


🌐 Internal & External Infrastructure Pentesting (with MITRE Mapping)
        •	📤 External Infrastructure Testing
                o	Goal: Assess attack surface from the internet
                o	Recon: Passive (OSINT, Shodan), Active (nmap, masscan, amass)
                o	Common targets: VPN gateways, web apps, SSH, RDP, email servers
                o	Vulnerability identification: CVE scans, unauthenticated endpoints
                o	Exploitation: Public exploits, password spraying, credential reuse
                o	Web fingerprinting: httpx, whatweb, wafw00f
                o	Cloud perimeter enumeration (S3 buckets, Azure, GCP exposed services)
                o	MITRE ATT&CK Mapping:
                        o	Initial Access: T1190 (Exploit Public-Facing Application), T1078 (Valid Accounts)
                        o	Discovery: T1046 (Network Service Scanning)
                        o	Credential Access: T1110 (Brute Force)
        •	🏠 Internal Infrastructure Testing
                o	Goal: Simulate attacker with internal network access
                o	Entry: VPN access, LAN drop, rogue device, insider threat
                o	Enumeration:
                        o	Active Directory (BloodHound, ldapsearch, powerview)
                        o	Shares (enum4linux, smbclient, crackmapexec)
                        o	Host discovery (ping sweep, arp scan, nbtscan)
                        o	Services: MSSQL, RDP, SMB, RPC
                o	Lateral Movement:
                        o	Pass-the-Hash, Pass-the-Ticket, Kerberoasting
                        o	PsExec, WMI, WinRM
                o	Privilege Escalation:
                        o	Local exploits (Windows, Linux)
                        o	Misconfigured services, stored credentials
                o	Credential Dumping:
                        o	mimikatz, lsassy, procdump + sekurlsa
                o	MITRE ATT&CK Mapping:
                        o	Discovery: T1087 (Account Discovery), T1018 (Remote System Discovery)
                        o	Credential Access: T1003 (OS Credential Dumping)
                        o	Lateral Movement: T1021 (Remote Services)
                        o	Privilege Escalation: T1068 (Exploitation for Privilege Escalation)
        •	🧾 Deliverables & Documentation
                o	Network topology map (if available)
                o	Inventory of discovered systems and services
                o	Vulnerability list with CVSS and evidence
                o	Exploited paths and impact assessment
                o	MITRE correlation to each phase
                o	Screenshots, payloads used, logs
                o	Remediation recommendations
                o	Executive summary and technical deep dive


📄 Structure of a Penetration Testing Report
        •	🧾 1. Cover Page
                o	Client name, logo, and project title
                o	Report title (e.g., “Web Application Penetration Test Report”)
                o	Date of submission
                o	Test dates (start–end)
                o	Classification (e.g., Confidential)
                o	Test version and revision number
                o	Tester(s) name and contact
        •	📬 2. Letter of Engagement
                o	Overview of the engagement scope and duration
                o	Authorized contacts and project stakeholders
                o	Legal statement confirming permission to test
                o	Disclaimer of liability and usage of report
                o	Summary of rules of engagement (ROE)
        •	📊 3. Executive Summary
                o	Brief explanation of test type and goals
                o	General security posture of tested assets
                o	Summary of major findings (e.g., 3 Critical, 2 High, etc.)
                o	Overall risk level (Critical/High/Medium/Low)
                o	Business impact in simple, non-technical terms
                o	Short bullet list of top recommendations
        •	🔍 4. Methodology
                o	Testing frameworks used (PTES, OWASP, NIST)
                o	High-level overview of test phases:
                        o	Reconnaissance
                        o	Scanning & Enumeration
                        o	Exploitation
                        o	Post-exploitation
                        o	Reporting
                o	Testing approach (black-box, white-box, grey-box)
                o	Tools used (e.g., Nmap, Burp Suite, Metasploit, custom scripts)
        •	🗺 5. Scope
                o	List of in-scope targets:
                        o	IP ranges / domain names / subdomains
                        o	APIs / applications / servers / devices
                        o	Cloud resources (if applicable)
                o	Out-of-scope components
                o	Constraints or limitations (e.g., no DoS, limited time window)
                o	Environment context (Production, Staging, Isolated test)
        •	⚠ 6. Findings Overview Table
                o	Table with all discovered vulnerabilities:
                        o	ID / Title
                        o	Severity (Critical/High/Medium/Low/Info)
                        o	Affected asset(s)
                        o	CWE/CVSS reference
                        o	Page or function affected
                        o	Remediation status (Open / Closed / Accepted Risk)
        •	📌 7. Detailed Findings
        Each finding should include:
                o	Title: Clear and concise vulnerability name
                o	Severity: Risk rating (with justification)
                o	CVE/CWE ID (if applicable)
                o	Affected assets: IPs, domains, URLs
                o	Technical Description: Explain the vulnerability, how it works, and why it's a risk
                o	Evidence:
                        o	Steps to reproduce
                        o	Request/response pairs
                        o	Screenshots, logs, or extracted data
                o	Impact: Business and technical implications
                o	Remediation Recommendations:
                        o	Short-term fix
                        o	Long-term fix (e.g., architectural)
                        o	Reference links (e.g., OWASP, NIST)
        •	🔁 8. Retesting Results (if applicable)
                o	Table or section documenting:
                        o	Which findings were revalidated
                        o	Whether they were resolved or remain open
                        o	Date of retest and tester signature
        •	🧩 9. Appendices
                o	Tool outputs (e.g., Nmap, Nessus, sqlmap logs)
                o	Full request/response traces
                o	Command-line syntax used
                o	Hashes of critical files for integrity
                o	Diagrams of network or attack paths
                o	Proof-of-concept scripts (if allowed)
                o	Timeline of attack chain / kill chain
        •	🔐 10. Report Metadata & Integrity
                o	SHA256 hash of report PDF for verification
                o	Digital signature or PGP key (if applicable)
                o	Notes on confidential handling and destruction after use


📱 Mobile Application Penetration Testing
        •	📲 Goals & Scope
                o	Identify vulnerabilities in Android and iOS mobile apps
                o	Evaluate communication security, storage security, runtime protections
                o	Ensure apps comply with OWASP MASVS (Mobile App Security Verification Standard)
        •	⚙️ Environment Setup
                o	Android: Rooted emulator/device, Frida, jadx, objection, adb
                o	iOS: Jailbroken device/simulator, Frida, class-dump, cycript, idevicesyslog
                o	Tools: MobSF, Burp Suite, mitmproxy, Frida, apktool, Ghidra, Hopper
        •	🔍 Static Analysis (SAST)
                o	Decompiling APK/IPA
                o	Searching for hardcoded credentials/API keys
                o	Analyzing manifest/plist configurations
                        o	AndroidManifest.xml: exported components, permissions
                        o	iOS Info.plist: URL schemes, ATS configuration
                o	Signature verification, root/jailbreak checks
        •	🏃 Dynamic Analysis (DAST)
                o	Proxying app traffic (Burp, mitmproxy)
                o	SSL pinning bypass (Frida, Objection)
                o	Runtime hooking (Frida scripts, Cycript)
                o	Analyzing behavior during login, session, data storage
        •	🧠 Business Logic Testing
                o	Authentication/Authorization bypass
                o	Insecure direct object references (IDOR)
                o	Broken session management
                o	Mobile-specific abuse cases (intent manipulation, deep linking)
        •	🔐 Local Storage Security
                o	SharedPreferences, NSUserDefaults, SQLite DBs, internal files
                o	Detecting sensitive data at rest (tokens, PII)
                o	Encryption checks (AES, key obfuscation)
        •	🛰 Communication Security
                o	HTTP vs HTTPS, TLS configurations
                o	Certificate pinning, downgrade attacks
                o	Token leakage (headers, query params)
        •	🧩 Reverse Engineering & Tampering
                o	Instrumentation bypass
                o	Modifying app behavior (smali patching, Frida)
                o	Custom-built Frida scripts for bypassing checks
        •	🛑 Common Mobile Vulnerabilities (OWASP Mobile Top 10)
                o	M1: Improper Platform Usage
                o	M2: Insecure Data Storage
                o	M3: Insecure Communication
                o	M4: Insecure Authentication
                o	M5: Insufficient Cryptography
                o	M6: Insecure Authorization
                o	M7: Client Code Quality Issues
                o	M8: Code Tampering
                o	M9: Reverse Engineering
                o	M10: Extraneous Functionality
        •	📦 Deliverables
                o	Summary of findings mapped to MASVS and OWASP
                o	Screenshots and reproduction steps
                o	Burp logs, Frida scripts, modified APKs
                o	Risk assessment per issue (CVSS / custom rating)
                o	Remediation advice and secure design recommendations
                o	Executive summary and technical appendix


☁️ Cloud Penetration Testing
        •	☁️ Goals & Objectives
                o	Simulate attacks targeting cloud infrastructure and services
                o	Identify misconfigurations, weak IAM policies, and exploitable cloud components
                o	Evaluate security posture across SaaS, PaaS, and IaaS models
                o	Provide actionable remediation guidance
        •	🔧 Environment Setup & Access
                o	Target cloud providers: AWS, Azure, GCP
                o	Create test environments with various services (VMs, containers, storage, databases)
                o	Set up credentials with different roles (admin, user, developer)
                o	Define rules of engagement and scope
        •	🔍 Reconnaissance & Enumeration
                o	DNS enumeration for cloud domains and subdomains
                o	Identifying services: S3 buckets, Azure Blobs, Google Storage
                o	Passive recon using OSINT (e.g., GitHub, Google dorks, crt.sh)
                o	Tools: Amass, Subfinder, CloudEnum, S3Scanner
        •	🛡 IAM Misconfiguration Testing
                o	Identify overprivileged roles and users
                o	Misconfigured policies and permission boundaries
                o	Exploiting AssumeRole and trust relationships
                o	Enumeration with tools: ScoutSuite, PMapper, IAM Vulnerable Policies
                o	Privilege escalation paths (e.g., attaching policies, lambda abuse)
        •	🔓 Public Cloud Storage & Database Exposure
                o	Check for publicly accessible S3, Azure Blobs, and GCP Buckets
                o	Enumeration of misconfigured DBs (MongoDB, Elasticsearch, Redis)
                o	Data extraction and access testing
        •	⚙️ Service-Specific Exploitation
                o	AWS
                        o	Lambda privilege escalation
                        o	SSRF on EC2 metadata
                        o	Misused IAM roles and STS
                        o	Secrets Manager and Parameter Store leaks
                o	Azure
                        o	Azure AD abuse (e.g., password spray, token replay)
                        o	Exploiting Azure Functions and App Services
                        o	Azure Automation Runbooks
                o	GCP
                        o	IAM misconfiguration and privilege escalation
                        o	Exploiting Cloud Functions & metadata
                        o	Service account impersonation
        •	🛠 Containers in Cloud
                o	EKS, AKS, GKE cluster enumeration and exploitation
                o	Exposed dashboards (e.g., Kubernetes, Portainer)
                o	Container breakout techniques
                o	Misconfigured container roles and secrets
        •	🔍 Logging, Monitoring & Detection Evasion
                o	Analyze logging capabilities: AWS CloudTrail, Azure Monitor, GCP Cloud Logging
                o	Evade detection using obfuscation, proxychains, minimal privileges
                o	Detection of honeypots and decoys
        •	🧩 Post-Exploitation & Lateral Movement
                o	Enumerate cross-service relationships
                o	Use harvested credentials to access new targets
                o	Pivoting through serverless functions or identity impersonation
        •	📦 Deliverables
                o	Executive summary with risk ratings
                o	Technical findings with reproduction steps and screenshots
                o	Cloud architecture diagram with findings highlighted
                o	IAM and privilege graphs (e.g., PMapper)
                o	Remediation steps and cloud-specific hardening advice
                o	MITRE ATT&CK mapping for cloud-based techniques


🤖 Generative AI Attacks
        •	🧠 Introduction to Generative AI and LLMs
                o	What is Generative AI?
                o	Examples: GPT, Claude, Gemini, DALL·E, Midjourney
                o	Large Language Models (LLMs) and foundation models
                o	Difference between training, fine-tuning, and inference
                o	Typical use cases: chatbots, assistants, code generation, content creation
        •	🚨 Threat Landscape
                o	Trust boundaries in human-AI interaction
                o	Attack surfaces:
                        o	Prompt input field
                        o	API endpoints
                        o	Model training pipeline
                        o	Plugins and tools (agents)
                o	Public vs private models (open weights vs SaaS)
        •	📥 Prompt Injection Attacks
                o	Direct prompt injection
                o	Indirect prompt injection (via data sources, websites, files)
                o	Encoding and escaping techniques
                o	Bypassing safety filters / jailbreaks
                o	Examples of prompt injection in chatbots and copilots
        •	🧬 Training Data Poisoning
                o	Poisoning public datasets (GitHub, Stack Overflow, Wikipedia)
                o	Model skewing by injecting biased or malicious examples
                o	Detection difficulty and long-term risk
        •	🔓 Model Output Manipulation
                o	Data leakage from models (training data inference)
                o	Model hallucinations used maliciously
                o	Induced misinformation campaigns
                o	Evasion of guardrails and alignment controls
        •	🧑‍💻 Code Generation Vulnerabilities
                o	Insecure code generation by LLMs (e.g., SQL injection, path traversal)
                o	Overtrust by developers (copy/paste risk)
                o	Lack of contextual security validation
                o	Dependency confusion and package suggestion poisoning
        •	📡 Abuse of AI for Recon and Payload Generation
                o	Using LLMs for crafting payloads (phishing, malware evasion, obfuscated code)
                o	Natural language recon (e.g., domain-specific information gathering)
                o	Social engineering automation via personas
        •	⚙️ Model Abuse in Real-World Systems
                o	LLM-integrated APIs abused via crafted inputs
                o	Business logic manipulation
                o	Abuse of autonomous agents and AI decision-making pipelines
        •	🛡️ Defensive Measures
                o	Prompt validation and contextual isolation
                o	Rate limiting and prompt memory control
                o	Fine-tuned moderation layers
                o	Red teaming AI systems (e.g., Anthropic’s RHP, OpenAI’s alignment evals)
                o	LLM firewalls and pre-processing wrappers
        •	📚 Frameworks and Guidelines
                o	OWASP Top 10 for LLMs (2023 draft)
                o	NIST AI Risk Management Framework (RMF)
                o	Microsoft’s Responsible AI Standard
                o	AI Red Teaming playbooks
        •	🧪 Labs and Tools
                o	LLM-RedTeaming, Atheris, Gaia
                o	LangChainGuard, PromptBench
                o	GPT4 Jailbreak tracker repos
                o	Adversarial testing platforms for generative models


🖥️ Thick Client Application Penetration Testing
        •	🎯 Goals & Scope
                o	Identify vulnerabilities in desktop-based applications that interact with backend services
                o	Reverse engineer client logic and validate input handling
                o	Analyze network, file system, and memory interactions
        •	🛠 Environment Preparation
                o	Tools: Procmon, Wireshark, Burp Suite, Fiddler, Ghidra, x64dbg, .NET Reflector, PE Studio
                o	Install and sandbox application (e.g., Windows VM with snapshot rollback)
                o	Configure intercepting proxy (mitmproxy/Fiddler) and SSL pinning bypass techniques
        •	🔍 Static Analysis
                o	Identify application tech stack: .NET, Java, C++
                o	Extract strings and configurations from binaries
                o	Analyze hardcoded credentials/API keys, obfuscated logic
                o	Check for local database/storage usage (SQLite, local files, registry)
        •	🏃 Dynamic Analysis
                o	Monitor filesystem: read/write operations, config files, logs
                o	Network traffic inspection: HTTP/S, SOAP, RPC, proprietary protocols
                o	Intercepting and modifying requests to the backend
                o	Test for insecure direct object references, session flaws
        •	🧪 Business Logic & Functionality Testing
                o	Bypass client-side validations
                o	Abuse application workflows (e.g., privilege escalation, logic flaws)
                o	Analyze error messages and debug output for sensitive data leaks
        •	🔓 Authentication & Authorization Testing
                o	Credential storage in memory, file, registry
                o	Token/session hijacking through intercepted communications
                o	Role-based access validation (e.g., user vs admin views)
        •	🧠 Reverse Engineering
                o	Disassemble and analyze application logic
                o	Hook functions using Frida or dynamic instrumentation
                o	Patch binaries to disable protections (e.g., authentication, license checks)
        •	🛡 Anti-Reversing & Security Controls
                o	Detect and bypass anti-debugging, anti-tampering mechanisms
                o	Understand code obfuscation, packing techniques
        •	🔐 Common Vulnerabilities
                o	Local privilege escalation via insecure services
                o	Insecure cryptographic implementations
                o	Exposure of sensitive data via logs/config files
                o	Insecure update mechanisms (DLL hijacking, MITM updates)
        •	🧾 Deliverables
                o	Technical report with severity-ranked issues
                o	Reproduction steps and proof of concept (POC)
                o	Reverse engineering insights and control flow maps
                o	Screenshots of dynamic analysis findings
                o	Recommendations for patching and secure coding
                o	Executive summary for management


🔄 Reverse Engineering Fundamentals
        •	🎯 Purpose & Goals
                o	Understand how software works without source code
                o	Analyze compiled applications, malware, or unknown binaries
                o	Identify vulnerabilities, hidden features, and logic flaws
        •	🛠 Tools & Setup
                o	Disassemblers: Ghidra, IDA Pro, Binary Ninja
                o	Debuggers: x64dbg, WinDbg, OllyDbg
                o	Scripting tools: Frida, Radare2, Angr
                o	Environment: Isolated Windows/Linux VMs with snapshots
                o	PE/ELF analysis: PEStudio, CFF Explorer, Readelf
        •	🧱 Binary Formats
                o	Executable file types: PE, ELF, Mach-O
                o	Understanding headers, sections, imports/exports
                o	Static linking vs dynamic linking
        •	⚙️ Assembly Language Basics
                o	Registers (EAX, ECX, etc.), Stack, Instruction Pointer
                o	Common instructions: MOV, PUSH, POP, CALL, RET, JMP
                o	Calling conventions (cdecl, stdcall, fastcall)
                o	Function prologue/epilogue structure
        •	🧠 Control Flow Analysis
                o	Analyzing function trees and call graphs
                o	Understanding loops, conditionals, branches
                o	Control flow obfuscation techniques and de-obfuscation
        •	🐞 Debugging & Dynamic Analysis
                o	Setting breakpoints, stepping, tracing execution
                o	Memory analysis: heap, stack, registers
                o	Identifying and bypassing anti-debugging tricks
        •	🛡 Anti-Reversing Protections
                o	Packers and obfuscators
                o	Virtualized code and custom instruction sets
                o	Self-modifying code detection
        •	🧪 Malware Reverse Engineering
                o	Behavior analysis in sandboxed environments
                o	Network traffic inspection
                o	Extracting IOCs and identifying persistence mechanisms
                o	Signature vs behavioral-based detection
        •	🔐 Cryptographic Analysis
                o	Identifying crypto functions and algorithms
                o	Analyzing key handling and storage
                o	Detecting weak or custom encryption logic
        •	🧾 Deliverables
                o	Annotated disassembly or pseudocode
                o	Behavioral and functional summaries
                o	Indicators of compromise (IOCs)
                o	Technical report with reverse engineering insights
                o	Risk assessment and remediation guidance


🧾 Securety Code Review (Source Code Analysis)
        •	🎯 Purpose & Goals
                o	Identify security vulnerabilities in source code before production
                o	Understand the flow of data and control across the application
                o	Detect insecure coding practices and logic flaws
        •	🛠 Tools & Setup
                o	Static Analysis Tools: SonarQube, Checkmarx, Semgrep, Fortify, Brakeman
                o	Linters: ESLint, Pylint, RuboCop
                o	IDE plugins for inline detection: Visual Studio Code, IntelliJ
                o	Source control analysis (e.g., Git hooks, commit scanning)
        •	🧪 Common Vulnerability Categories to Identify
                o	Input validation issues (e.g., XSS, SQL Injection)
                o	Authentication and session management flaws
                o	Insecure file uploads and path traversal
                o	Cryptographic misuses (e.g., hardcoded keys, weak hashing)
                o	Insecure use of APIs/libraries
                o	Inadequate logging and error handling
                o	Race conditions and TOCTOU issues
                o	Business logic flaws (e.g., broken workflows, privilege escalation)
        •	🔍 Code Analysis Techniques
                o	Taint analysis: Track user input from source to sink
                o	Control flow analysis: Understand branching and edge cases
                o	Data flow tracing: Follow data transformations through variables/functions
                o	Manual review for sensitive areas: auth, crypto, file handling
        •	🔐 Secure Coding Standards
                o	OWASP Secure Coding Practices
                o	SEI CERT Coding Standards (C/C++, Java)
                o	Language-specific guidelines (e.g., .NET, Python, JavaScript)
        •	🧰 Automation & CI/CD Integration
                o	Integrate scanners into build pipelines (GitHub Actions, GitLab CI, Jenkins)
                o	Configure thresholds and break builds on high-severity findings
                o	Periodic re-scanning of codebases
        •	📂 Deliverables
                o	Vulnerability summary with severity levels and CWE references
                o	Annotated source code snippets showing vulnerable logic
                o	Recommendations for remediation and secure patterns
                o	Integration roadmap for secure coding and DevSecOps
                o	Executive summary for stakeholders


⚙️ CI/CD Security Processes
        •	🎯 Purpose & Relevance
                o	Secure the entire DevOps pipeline from design to deployment
                o	Reduce attack surface throughout the Software Development Life Cycle (SDLC)
                o	Shift security left – embed controls at the earliest development stages
        •	🧩 Phase 1: Design Review & Architecture Security
                o	Understand system architecture (e.g., client-server, microservices, cloud-native)
                o	Review threat modeling methodologies:
                        o	STRIDE
                        o	DREAD (less common today)
                        o	PASTA
                o	Analyze data flows and trust boundaries
                o	Identify assets, actors, entry points, and critical paths
                o	Document expected behavior and risk assumptions
        •	🛡 Phase 2: Threat Modeling
                o	Define attacker profiles and motivations
                o	Identify possible threats, misuse cases, and abuse cases
                o	Classify risks using CVSS or internal severity models
                o	Validate controls and propose mitigations
                o	Tools: Threat Dragon, OWASP Threat Modeling Cheat Sheet, Microsoft TMT
        •	🧪 Phase 3: Development Security Practices
                o	Secure coding guidelines based on language (e.g., .NET, Java, Python)
                o	Input validation and output encoding
                o	Error handling and secure logging
                o	Credential management and secret rotation
                o	API security: rate limiting, authentication, authorization
                o	Secure session management
        •	🔐 Phase 4: CI/CD Pipeline Hardening
                o	Tools: Jenkins, GitHub Actions, GitLab CI, CircleCI, Azure DevOps
                o	Enforce least privilege for runners and agents
                o	Protect secrets and environment variables using vaults (AWS Secrets Manager, Vault)
                o	Validate configurations using IaC scanning tools (Checkov, tfsec)
                o	Integrate software composition analysis (e.g., Snyk, OWASP Dependency-Check)
                o	Secure access to artifact registries (e.g., Nexus, Artifactory, GitHub Packages)
        •	🧰 Phase 5: Security Testing Integration
                o	Static Analysis (SAST): integrated in early commit/PR stages
                o	Dynamic Analysis (DAST): deployed against staging/pre-prod
                o	Interactive App Security Testing (IAST) for runtime code monitoring
                o	IaC scanning for Terraform, Helm, Kubernetes manifests
                o	Container image scanning: Trivy, Grype, Clair
        •	🧮 Phase 6: Security Automation & Orchestration
                o	Auto-fix PR suggestions via security bots
                o	Pull request gates: block merges if critical issues found
                o	ChatOps: push alerts to Slack/MS Teams
                o	DevSecOps ticketing integration with Jira, Azure Boards
                o	Weekly security trend reports per repo/team
        •	📦 Deliverables & Documentation
                o	End-to-end CI/CD threat model diagrams
                o	Full pipeline map: tools, runners, secrets, access levels
                o	Inventory of third-party dependencies and security reviews
                o	Report of scanning tool results, risk ratings, and remediations
                o	Executive summary for management on DevSecOps maturity
                o	Timeline of implementation and security improvements


📡 Wi-Fi Penetration Testing
        •	🔍 Objective
                o	Identify and exploit security weaknesses in wireless networks
                o	Evaluate network segmentation, authentication, and encryption practices
        •	🧱 Foundational Concepts
                o	Wi-Fi Standards: IEEE 802.11a/b/g/n/ac/ax
                o	Frequency Bands: 2.4 GHz vs 5 GHz vs 6 GHz (Wi-Fi 6E)
                o	Modulation Techniques: OFDM, DSSS
                o	Channels and Interference
                o	Signal Strength, Range, and Coverage
        •	🔒 Security Protocols
                o	WEP: Weak and deprecated
                o	WPA/WPA2-Personal: PSK-based, vulnerable to offline brute-force
                o	WPA/WPA2/WPA3-Enterprise: Uses 802.1X and RADIUS
                o	EAP Methods: EAP-TLS, PEAP, EAP-TTLS
                o	PMF (Protected Management Frames)
        •	🛠 Tools & Setup
                o	Wireless NICs supporting monitor mode and packet injection (e.g., Alfa cards)
                o	Kali Linux with aircrack-ng suite
                o	Wireshark for packet capture and analysis
                o	Bettercap for real-time attacks
                o	hcxdumptool + hashcat for WPA cracking
                o	Kismet and Airodump-ng for discovery
        •	🧪 Reconnaissance Phase
                o	Scanning networks and APs (SSID, BSSID, channel, encryption)
                o	Identifying clients (stations) associated with APs
                o	Monitoring beacon frames, probe requests, authentication requests
        •	🎯 Attack Scenarios
                o	Passive Capture + Dictionary Attack on WPA2
                o	Deauthentication attack to capture WPA handshake
                o	Rogue Access Point / Evil Twin
                o	Karma attack (auto-connect exploitation)
                o	Captive Portal Phishing (DNS Spoof + Custom Login Page)
                o	EAP Downgrade Attack
                o	PMKID Hash Extraction
        •	⚙️ Enterprise Network Attacks
                o	Capturing MSCHAPv2 (PEAP) authentication traffic
                o	Using tools like eaphammer for evil twin + auth capture
                o	Cracking challenge-response for NTLM hashes
                o	Relaying credentials to access AD services
        •	🧱 Infrastructure Assessment
                o	AP misconfiguration (open SSIDs, fallback auth, dual modes)
                o	Client-side attacks via Wi-Fi pineapple or malicious APs
                o	Segmentation and isolation testing (client-to-client traffic)
                o	Hidden SSIDs and probe response enumeration
        •	🧾 Deliverables
                o	Wireless environment topology map
                o	Detailed attack paths and captured handshakes/logs
                o	Screenshots of successful attacks (e.g., WPA2 handshake, Evil Twin portal)
                o	Recommendations: encryption improvements, MAC filtering, AP isolation, EAP config
                o	Risk rating based on potential access (e.g., internal network pivot)
                o	Suggested detection mechanisms (WIDS/WIPS, log analysis)


📻 RF (Radio Frequency) Security Testing
        •	🎯 Objective
                o	Assess and exploit vulnerabilities in RF-based technologies (beyond Wi-Fi)
                o	Evaluate custom protocols, hardware transmissions, and security mechanisms
        •	🧠 Fundamentals of RF Communication
                o	Analog vs Digital Signals
                o	Frequency Spectrum: LF, HF, VHF, UHF, ISM bands
                o	Modulation Types: AM, FM, ASK, FSK, PSK, GFSK
                o	Bandwidth, latency, and signal-to-noise ratio
                o	Channel separation and interference considerations
        •	📡 Common RF Technologies
                o	Bluetooth & BLE
                o	Zigbee & Z-Wave
                o	LoRa & LoRaWAN
                o	RFID & NFC
                o	Proprietary RF remotes and sensors (e.g., car fobs, alarms)
                o	Satellite and radio broadcast
                •	🛠 Hardware and Tools
                o	SDR (Software Defined Radio): HackRF One, RTL-SDR, USRP
                o	Antennas: directional, omnidirectional, Yagi
                o	RF spectrum analyzer (hardware or software-based)
                o	Tools: GQRX, SDR#, GNURadio, URH (Universal Radio Hacker), BladeRF
                o	Protocol-specific analyzers: BTLEJack, KillerBee (Zigbee), Proxmark3 (RFID)
        •	🔍 Reconnaissance
                o	Signal sniffing with SDR tools
                o	Identifying frequency and bandwidth of target device
                o	Capturing unknown protocols
                o	Reversing raw RF data and replay structure
                o	Differentiating legitimate vs rogue signals
        •	🧪 Attack Techniques
                o	Replay attacks on RF-controlled devices (e.g., garage openers, alarms)
                o	Signal jamming and DoS on specific frequencies
                o	Man-in-the-Middle (MiTM) on BLE/Zigbee using rogue devices
                o	Brute-force of access codes in RF-controlled systems
                o	Side-channel leakage detection (e.g., TEMPEST-style leaks)
        •	🧱 Specialized Scenarios
                o	Breaking NFC payment flows using Proxmark3
                o	Extracting keys from RFID (e.g., MIFARE Classic key cracking)
                o	Attacks against LoRaWAN: Join/Leave manipulation, key re-use
                o	BLE spoofing with BTLEJack or BlueZ stack abuse
                o	Zigbee sniffing, injection, and impersonation with KillerBee
        •	📦 Deliverables
                o	Mapping of RF devices in environment with frequency/technology use
                o	Recorded transmissions and decoded payloads (where applicable)
                o	Screenshots or logs from signal capture and attack stages
                o	Recommendations for RF shielding, protocol hardening, and signal isolation
                o	Risk rating per device or protocol used
                o	RF spectrum assessment log and interference footprint


🧷 Hardware Penetration Testing
        •	🧭 Introduction to Hardware Hacking
                o	What is hardware penetration testing?
                o	Goals: data extraction, bypass protections, physical compromise
                o	Typical targets: routers, IoT, embedded devices, ATMs, POS
                o	Legal and ethical considerations
                o	Required lab equipment and safety
        •	🔌 Physical Interface Discovery & Access
                o	Identifying debugging interfaces (UART, JTAG, SPI, I2C)
                o	Locating test points and headers
                o	Pinout mapping with multimeter / logic analyzer
                o	Interfacing with:
                        o	UART (via USB-TTL converters)
                        o	SPI flash chips (via SOIC clip)
                        o	JTAG (via JTAGulator, OpenOCD)
                o	Chip-off techniques and desoldering
        •	📡 RF and Wireless Communication Analysis
                o	Common protocols: Bluetooth, Zigbee, LoRa, Sub-GHz, NFC, RFID
                o	SDR tools: HackRF, RTL-SDR, Flipper Zero, Yard Stick One
                o	Signal capture and replay attacks (GQRX, Universal Radio Hacker)
                o	Rolling code vs static code systems
                o	Side-channel attacks: EM leakage, power analysis 
        •	💾 Firmware Extraction & Analysis
                o	Dumping firmware from flash chips (e.g., SPI NOR)
                o	Firmware formats: bin, hex, ELF, squashfs, uImage
                o	Tools: Binwalk, Firmware Mod Kit, Ghidra, QEMU, Cutter
                o	Reconstructing file systems
                o	Identifying credentials, hardcoded keys, and backdoors
                o	Signature and integrity validation bypass
        •	🧠 Reverse Engineering & Debugging
                o	Identifying microcontrollers (MCU) and chipsets
                o	Reading datasheets and identifying pinout
                o	Using IDA Pro / Ghidra for disassembly
                o	Tracing function calls and memory access
                o	Emulating firmware for dynamic analysis
        •	🔐 Bypassing Protections
                o	UART shell drop and serial console login
                o	Bootloader exploitation (U-Boot, CFE)
                o	Logic flaws in update mechanism
                o	Password reset via flash modification
                o	NAND / NOR mirroring and tamper detection bypass
        •	🧰 Tools & Equipment
                o	Multimeter, oscilloscope, soldering iron, hot air station
                o	USB analyzers, logic analyzers
                o	SOIC clips, breakout boards
                o	Bus Pirate, JTAGulator, Saleae Logic
                o	Flipper Zero, Proxmark3, HackRF One
                o	3D-printed enclosures and probe holders
        •	🧪 Lab Setup & Workflow
                o	Safe device disassembly
                o	Isolation and anti-static precautions
                o	Documentation and photography
                o	Labeling connections and pinouts
                o	Working with partially functional devices
                o	Tracking modifications
        •	🧠 Real-World Scenarios
                o	IoT device bootloader bypass
                o	ATM firmware extraction and tamper detection
                o	Consumer router shell access via UART
                o	Smart lock replay attack over BLE
                o	Embedded Linux root access via soldered SPI
        •	📋 Reporting & Deliverables
                o	Physical evidence photos (PCB, wiring, ports)
                o	Firmware hashes, extracted secrets
                o	Attack narrative with diagrams
                o	Vulnerability descriptions and CVSS scores
                o	Suggested mitigations (encryption, secure boot, fuse settings)
                o	Recommendations for future designs


🦠 Malware Analysis
        •	🔍 Introduction to Malware Analysis
                o	What is malware?
                o	Types of malware:
                        o	Virus
                        o	Worm
                        o	Trojan
                        o	Ransomware
                        o	Spyware
                        o	Rootkits
                        o	Keyloggers
                        o	Fileless malware
                o	Malware lifecycle and objectives
                o	Common infection vectors (phishing, drive-by, USB)
        •	🧪 Types of Malware Analysis
                o	Static Analysis
                        o	Hashing (MD5, SHA1, SHA256)
                        o	File type and structure (PE, ELF, APK, DOCX)
                        o	String extraction (strings, FLOSS)
                        o	Disassembly (IDA, Ghidra, Radare2)
                        o	YARA rule creation
                        o	Detecting packers and obfuscation (PEiD, Detect It Easy)
                o	Dynamic Analysis
                        o	Behavior monitoring in sandbox (Cuckoo, Any.Run, Joe Sandbox)
                        o	Process creation and injection
                        o	Network communication
                        o	Registry and file system modifications
                        o	API call tracing (ProcMon, API Monitor)
                o	Hybrid Analysis
                        o	Combining static and dynamic analysis
                        o	Automation with tools and sandbox correlation
        •	🛠️ Malware Analysis Lab Setup
                o	Air-gapped or isolated VMs
                o	Recommended software:
                        o	Windows XP/7/10 VM
                        o	Linux VM (for command-line analysis)
                        o	Tools: x64dbg, Wireshark, Procmon, Process Hacker, Autoruns
                o	Snapshots and rollback
                o	Network simulation tools (INetSim, Fakenet-NG)
                o	Controlled DNS and internet access
        •	🧬 Executable Formats & Internals
                o	Windows PE format
                        o	Headers, sections (.text, .rdata, .rsrc)
                        o	Import Address Table (IAT)
                        o	Export Table
                        o	Entry point and packing indicators
                o	Linux ELF format basics
                o	Android APK structure
        •	🧠 Behavioral Analysis Techniques
                o	Registry changes (Autoruns, Regshot)
                o	File system interactions (Procmon, Filemon)
                o	Process and thread activity (Process Explorer)
                o	Network traffic (Wireshark, TCPView)
                o	Mutex and named pipe detection
        •	🕵️ Reverse Engineering for Malware
                o	Recognizing common functions and patterns
                o	Analyzing API calls (WinAPI, Kernel32, Ntdll)
                o	Control flow graphs
                o	Deobfuscation strategies
                o	Shellcode analysis and emulation
                o	Anti-debugging techniques and bypasses
        •	🧱 Persistence & Evasion Techniques
                o	Startup folder, Run keys, Scheduled Tasks
                o	DLL injection, Process hollowing
                o	Reflective DLL loading
                o	Code injection techniques
                o	UAC bypass methods
                o	AV/EDR evasion (encryption, obfuscation, LOLBins)
        •	🌐 Command and Control (C2)
                o	Beaconing behavior
                o	Protocols used: HTTP(S), DNS, ICMP, custom
                o	C2 domain identification and decoding
                o	Hardcoded IPs and domain generation algorithms (DGA)
        •	🧰 Advanced Tools and Techniques
                o	IDA Pro / Ghidra / Binary Ninja
                o	Dynamic instrumentation (Frida, Pin)
                o	Emulators and sandboxing
                o	Debugging packed binaries
                o	Heuristics and anomaly detection
        •	📋 Deliverables and Reporting
                o	Malware family identification
                o	Indicators of Compromise (IOCs): hashes, domains, IPs, mutexes
                o	Behavior summary and TTPs
                o	MITRE ATT&CK mapping
                o	Screenshots of execution and network traffic
                o	Recommendations and remediation actions


🛡️ Security Operations Center (SOC)
        •	🏢 SOC Fundamentals
                o	Purpose and role of a SOC
                o	Types of SOCs: Internal, Managed (MSSP), Hybrid
                o	SOC tiers and responsibilities (Tier 1, Tier 2, Tier 3, Threat Hunting)
                o	Common SOC roles: Analyst, Incident Responder, Engineer, Threat Hunter, Manager
        •	🧰 Core SOC Tools
                o	SIEM (Security Information and Event Management)
                        o	Examples: Splunk, QRadar, Sentinel, LogRhythm
                        o	Use cases: log collection, correlation rules, dashboards
                o	SOAR (Security Orchestration, Automation, and Response)
                        o	Playbooks and automation
                        o	Examples: Cortex XSOAR, Splunk SOAR
                o	EDR (Endpoint Detection and Response)
                        o	Examples: CrowdStrike, SentinelOne, Carbon Black
                        o	Threat detection and containment
                o	IDS/IPS (Intrusion Detection/Prevention Systems)
                        o	Signature vs. anomaly-based
                        o	Tools: Suricata, Snort
                o	Threat Intelligence Platforms
                        o	Feeds and enrichment sources (AlienVault OTX, MISP, VirusTotal)
                o	Asset inventory and vulnerability management
                        o	Tools: Qualys, Tenable, Rapid7
        •	🔍 Security Monitoring & Detection
                o	Log sources:
                        o	Windows Event Logs
                        o	Firewall logs
                        o	DNS logs
                        o	VPN logs
                        o	Proxy and web traffic logs
                o	MITRE ATT&CK for detection use cases
                o	Behavioral analytics and anomaly detection
                o	False positives and alert tuning
                o	KPIs and metrics for SOC efficiency
        •	🚨 Incident Response Process
                o	Detection and validation
                o	Triage and prioritization
                o	Containment (host, network, credentials)
                o	Investigation and root cause analysis
                o	Eradication and recovery
                o	Post-incident review and reporting
        •	🧪 Threat Hunting
                o	Hypothesis-driven hunting
                o	Hunting via logs, EDR data, and network flows
                o	Indicators of Attack (IOA) vs. Indicators of Compromise (IOC)
                o	Leveraging MITRE ATT&CK for hunts
        •	📋 SOC Reporting & Documentation
                o	Incident documentation
                o	Daily briefings and shift handovers
                o	Executive summaries
                o	Threat landscape reports
        •	🛡️ Blue Team Skills and Challenges
                o	Log analysis techniques
                o	Packet analysis
                o	Malware triage
                o	Memory analysis basics
                o	Threat emulation and purple teaming
                o	Common attacker techniques and detection strategies
        •	🧠 SOC Training & Simulation
                o	Using lab environments (e.g., DetectionLab, Security Onion)
                o	Capture The Flag (CTF) exercises
                o	Simulated attacks (Atomic Red Team, Caldera, MITRE ATT&CK Evaluations)


📜 Governance, Risk, and Compliance (GRC)
        •	📘 Foundations of GRC
                o	Definitions: Governance, Risk Management, Compliance
                o	Importance of GRC in cybersecurity and business
                o	GRC roles and responsibilities in an organization
                o	Integrating GRC into the security lifecycle
        •	📑 Governance
                o	Security policies and procedures
                o	Security frameworks (NIST CSF, ISO 27001, CIS Controls)
                o	Organizational structure and responsibility matrices (RACI)
                o	Data governance and ownership
                o	Policy lifecycle management
        •	⚖️ Risk Management
                o	Risk identification techniques (interviews, questionnaires, technical scans)
                o	Risk assessment methodologies (Qualitative vs. Quantitative)
                o	Risk treatment and mitigation strategies
                o	Risk register and continuous monitoring
                o	Business Impact Analysis (BIA)
                o	Third-party and supply chain risk management
        •	📋 Compliance
                o	Overview of common standards and regulations:
                        o	ISO/IEC 27001, NIST 800-53/171, SOC 2, PCI-DSS, HIPAA, GDPR, DORA
                o	Compliance audits and gap assessments
                o	Control mapping and inheritance
                o	Maintaining audit trails and evidence
                o	Role of compliance automation tools (Drata, Vanta, Tugboat Logic)
        •	🧰 GRC Tools and Platforms
                o	GRC platforms: ServiceNow GRC, RSA Archer, LogicGate
                o	Compliance tracking dashboards
                o	Policy and document management tools
                o	Risk scoring and visualization tools
        •	📈 Metrics and Reporting
                o	Key Risk Indicators (KRIs)
                o	Key Performance Indicators (KPIs)
                o	Security posture dashboards
                o	Risk heat maps and compliance scorecards
        •	🧠 GRC in Practice
                o	Real-world use cases of GRC implementation
                o	Aligning GRC with business goals
                o	Creating a culture of compliance
                o	Communicating GRC insights to executives
        •	🔄 Continuous Improvement
                o	Feedback loops from incidents and audits
                o	Control testing and validation
                o	Updating policies with lessons learned
                o	Integrating GRC with DevSecOps workflows



🔍Digital Forensics & Incident Response (DFIR)
        •	🧭 Introduction to DFIR
                o	Definition and scope of Digital Forensics and Incident Response
                o	Differences between forensics and incident response
                o	When and why DFIR is needed
                o	Legal and ethical considerations
                o	Chain of custody and evidence admissibility
        •	💾 Digital Forensics Fundamentals
                o	Types of digital evidence
                o	Sources: memory, disk, network, mobile, cloud
                o	Data acquisition techniques:
                        o	Bit-by-bit imaging (dd, FTK Imager, Guymager)
                        o	Live vs. dead acquisition
                        o	Write blockers and anti-forensics
                o	Forensic tools overview:
                        o	Autopsy, FTK, EnCase, X-Ways
                        o	Volatility, Sleuth Kit, Plaso (log2timeline)
                o	File systems: NTFS, FAT32, EXT4, APFS
                o	Recovering deleted files and partitions
        •	🔬 Memory Forensics
                o	Importance of RAM acquisition
                o	Tools: Volatility, Rekall
                o	Extracting:
                        o	Running processes
                        o	Open network connections
                        o	Loaded DLLs
                        o	Injected code and anomalies
                        o	Credential artifacts (LSASS)
        •	🖥️ Disk & File System Analysis
                o	Metadata and timestamps (MACB)
                o	Hidden partitions and slack space
                o	File carving techniques
                o	Identifying suspicious files:
                        o	File signatures
                        o	Hash comparisons (NSRL, VirusTotal)
                        o	Alternate Data Streams (ADS)
        •	🌐 Network Forensics
                o	Capturing network traffic (pcap, tcpdump, Wireshark)
                o	Protocol analysis (HTTP, SMB, DNS, etc.)
                o	Session reconstruction
                o	Identifying C2 traffic and data exfiltration
                o	Correlation with endpoint activity
        •	📱 Mobile & Cloud Forensics
                o	Android and iOS forensic approaches
                        o	Logical, file system, physical acquisition
                        o	Tools: Cellebrite, Magnet AXIOM, MOBILedit
                o	Cloud forensics:
                        o	AWS, Azure, GCP log analysis
                        o	API-based evidence acquisition
                        o	Legal jurisdiction and challenges
        •	🚨 Incident Response Process
                o	Preparation:
                        o	IR plan, playbooks, roles and responsibilities
                        o	Logging, alerting, and communication strategies
                o	Identification
                        o	Alerts and indicators of compromise (IOCs)
                        o	Triage tools and methods
                o	Containment
                        o	Isolating affected systems
                        o	Short-term vs. long-term containment
                o	Eradication
                        o	Malware removal
                        o	Patching vulnerabilities
                o	Recovery
                        o	System restoration and monitoring
                        o	Validating normal operations
                o	Lessons Learned
                        o	Root cause analysis
                        o	Reporting and documentation
                        o	Improving defenses
        •	🧪 Incident Types and Use Cases
                o	Ransomware attacks
                o	Business Email Compromise (BEC)
                o	Web server compromise
                o	Insider threats
                o	Credential theft and reuse
                o	Supply chain attacks
        •	🧰 Incident Response Tools
                o	Triage: Velociraptor, KAPE, GRR Rapid Response
                o	Memory capture: DumpIt, winpmem
                o	Analysis: ELK Stack, Splunk, MISP
                o	Forensics suites: Autopsy, SIFT Workstation
                o	Threat intel enrichment: VirusTotal, AbuseIPDB
        •	🧠 MITRE ATT&CK & DFIR
                o	Mapping adversary behavior to ATT&CK techniques
                o	TTP identification and trend analysis
                o	Integration into detection and response workflows
        •	📋 Reporting and Documentation
                o	Evidence log and preservation chain
                o	Timeline of events and indicators
                o	Executive summaries
                o	Detailed forensic findings
                o	Recommendations and preventive controls
