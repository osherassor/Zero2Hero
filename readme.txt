📦 PC Architecture & Hardware
    •	🧩 CPU (Central Processing Unit)
        o	Understand the purpose of the CPU
        o	Learn about Instruction Cycle: Fetch → Decode → Execute → Write Back
        o	Explore CPU Components:
            	ALU (Arithmetic Logic Unit)
            	Control Unit
            	Registers (general-purpose, special-purpose)
            	Cache (L1, L2, L3)
        o	Compare CPU Architectures:
            	x86, x64 (Intel/AMD)
            	ARM architecture
        o	Concepts of Multi-core and Hyper-Threading
        o	Clock speed vs performance
        o	CPU virtualization support (VT-x, AMD-V)
        o	Power consumption and thermal design
        o	Tools to monitor CPU usage and temperature
    •	📏 RAM (Random Access Memory)
        o	Understand the purpose of RAM (volatile memory)
        o	Learn about RAM types:
            	DDR3, DDR4, DDR5
            	ECC vs non-ECC
            	DIMM vs SO-DIMM
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
            	SATA, IDE, M.2, PCIe
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
            	CPU socket
            	RAM slots
            	VRM (Voltage Regulator Modules)
            	CMOS battery
        o	Buses:
            	Data, Address, Control
            	PCIe lanes and bandwidth
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
            	24-pin ATX
            	8-pin CPU
            	PCIe power
            	Molex, SATA power
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
            	Air cooling (fans, heatsinks)
            	Liquid cooling (AIO, custom loop)
            	Phase-change cooling (advanced)
        o	Thermal paste types and application
        o	Importance of airflow and case design
        o	Fan curves and noise optimization
        o	Temperature monitoring tools (HWMonitor, OpenHardwareMonitor)
        o	BIOS/UEFI fan control settings
        o	Thermal throttling behavior
        o	GPU-specific cooling systems
    •	🧩 Expansion & Peripherals
        o	Peripheral connection types:
            	USB (2.0/3.0/3.2/Type-C)
            	Bluetooth, PS/2, Thunderbolt
        o	Input Devices: keyboard types, mouse DPI, scanners
        o	Output Devices: monitor refresh rate, printers
        o	Expansion cards:
            	GPUs, sound cards, capture cards
            	Network cards (Wi-Fi, Ethernet)
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
            	Decimal → Binary
            	Binary → Decimal
            	Binary → Hexadecimal
        o	Signed vs unsigned numbers
        o	Two's complement
        o	Endianness: little-endian vs big-endian
        o	Floating-point representation (IEEE 754)
        o	Binary arithmetic: addition, subtraction, multiplication
        o	Bitwise operations:
            	AND, OR, NOT, XOR
            	Bit shifting (<<, >>)
        o	Bit masking and flag fields
        o	Representing negative numbers and overflows
    •	⚖️ Boolean Algebra & Logic Gates
        o	Boolean variables and logic expressions
        o	Truth tables and logic evaluation
        o	Fundamental logic gates:
            	AND, OR, NOT
        o	Derived gates:
            	NAND, NOR, XOR, XNOR
        o	De Morgan's Laws
        o	Combinational logic
        o	Minimizing logic expressions (Karnaugh Maps)
        o	Logic circuit simulation tools
        o	Logic propagation delays
        o	Using Boolean logic in control flow (if/else, conditions)
    •	🛠️ Digital Components
        o	Flip-Flops:
            	SR, D, JK, T Flip-Flops
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
            	Moore vs Mealy models
        o	Designing FSMs:
            	State diagrams
            	State transition tables
        o	Applications in digital design
        o	Use in protocol parsing
        o	Timing diagrams and delays
        o	HDL-based implementation (optional advanced)
        o	Clock synchronization
        o	Metastability issues in hardware
    •	🔹 Logic Implementation Tools
        o	Schematic vs text-based design
        o	Digital circuit simulators:
            	Logisim
            	CircuitVerse
            	Digital Works
        o	HDL introduction:
            	Verilog vs VHDL (basics only)
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
            	/etc – system config
            	/home – user directories
            	/var – variable files/logs
            	/usr – user binaries, libraries
            	/bin, /sbin, /lib, /lib64
            	/dev, /proc, /sys, /run
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
                        	Historical topologies: Token Ring, Bus
                        	Modern topologies: Star, Mesh, Tree, Hybrid
                o	Network Models
                        	OSI Model
                        	TCP/IP Stack
                o	Network Performance Metrics
                        	Latency, Jitter, Bandwidth, Throughput
                        	MTU, MSS
                o	Broadcast Domain vs Collision Domain
                        	Definitions, diagrams, and simulations
                        	Switch segmentation and VLAN boundaries
                        	Real-world implications in network design
                o	Message Types: Unicast, Broadcast, Multicast
                        	Layer 2: MAC unicast, multicast (01:00:5E), broadcast (FF:FF:FF:FF:FF:FF)
                        	Layer 3: IP unicast, broadcast (255.255.255.255), multicast (224.0.0.0/4)
                        	IGMP and multicast group management
                        	ARP and DHCP as broadcast examples
                        	DNS as unicast example
                        	Practical packet captures using Wireshark
    •	🧱 Networking Devices (Extended)
                o	Routers
                        	Static vs dynamic routing
                        	Default routes
                        	CIDR and summarization
                o	Switches
                        	Spanning Tree Protocol (STP, RSTP, MSTP)
                        	MAC learning and port forwarding decisions
                        	VLAN trunking (802.1Q)
                        	Switchport security features
                o	Hubs vs Switches
                        	Historical role of hubs
                        	Why switches replaced hubs
                        	Collision domains in hub networks
                        	Packet flooding vs MAC-based forwarding
                        	Demo lab: Sniffing on a hub vs switch
                o	NICs and Interfaces
                        	Promiscuous mode
                        	Duplex mismatch issues
                        	Auto-negotiation
                o	Firewalls
                        	Deep Packet Inspection (DPI)
                        	Zone-based firewall logic
                        	Common vendor CLI: Cisco ASA, Palo Alto
                o	Load Balancers
                        	Algorithms: Round-robin, least connections
                        	Health checks
                        	Application awareness (SSL termination)
                o	Wireless Infrastructure
                        	SSIDs, channels, encryption (WEP, WPA2, WPA3)
                        	2.4 GHz vs 5 GHz vs 6 GHz bands
                        	Access Point roles (controller-based, standalone)
                o	Modems and Gateways
                        	DSL, Cable, Fiber modems
                        	NAT behavior in gateways
                        	Dual NAT and CGNAT explained
    •	🏗️ OSI Model Layers (Expanded)
                o	Physical Layer
                        	Cable standards: Cat5e, Cat6, Cat6a, Cat7
                        	Fiber optic types: single-mode, multi-mode
                        	Signal degradation and attenuation
                        	Bit-level transmission simulation
                o	Data Link Layer
                        	Ethernet frame breakdown: Preamble, SFD, MACs, Type, FCS
                        	Switch loop protection (STP, BPDU Guard)
                        	VLAN tagging and double tagging (Q-in-Q)
                        	MAC flooding attacks (brief intro)
                o	Network Layer
                        	IPv4 fragmentation and reassembly
                        	Subnetting techniques and exercises
                        	Route redistribution concepts
                        	NAT types (static, dynamic, PAT)
                        	Layer 3 ACLs and firewalling
                o	Transport Layer
                        	TCP handshake deep dive (SYN, SYN-ACK, ACK)
                        	Retransmission and sliding window mechanics
                        	UDP with practical examples: TFTP, SNMP
                        	Port scans: SYN, FIN, NULL, Xmas (not exploitative yet)
                o	Session Layer
                        	SSL/TLS handshake overview
                        	RDP, SMB session creation
                o	Presentation Layer
                        	Data transformation: ASCII vs Unicode
                        	SSL/TLS encryption examples
                o	Application Layer
                        	HTTP headers: Host, Cookie, User-Agent
                        	DNS record types: A, AAAA, CNAME, MX, TXT
                        	DHCP options and packet flow (DORA)
                        	FTP active vs passive mode
                        	SMTP, IMAP, POP3 comparison

🔐 Security Basics
        •	🛡️ Foundations of Security
                o	What is Information Security?
                        	Confidentiality, Integrity, Availability (CIA Triad)
                        	Non-repudiation and Authentication
                        	Real-world examples of CIA violations
                o	Security Terminology
                        	Asset, Threat, Vulnerability, Exploit, Risk, Control
                        	Threat actor types: script kiddies, insiders, nation-states, APTs
                o	Security Principles
                        	Least privilege
                        	Defense in depth
                        	Fail-safe defaults
                        	Separation of duties
                        	Security through obscurity (debate)
                o	Types of Controls
                        	Physical, Administrative, Technical
                        	Preventive, Detective, Corrective, Deterrent, Recovery
                o	Security Domains
                        	Physical security
                        	Network security
                        	Application security
                        	Endpoint security
                        	Data security
                        	Identity and access management
                        	Cloud security (relation to cloud foundations)
        •	🔍 Vulnerabilities & Exposure
                o	Common vulnerabilities
                        	Misconfigurations
                        	Unpatched systems
                        	Weak credentials
                        	Insecure defaults
                        	Lack of encryption
                o	Public databases
                        	CVE, CVSS scoring
                        	NVD, Exploit DB (overview only)
                o	Security misconfigurations examples
                        	Directory listing
                        	Default credentials
                        	Unrestricted ports/services
                o	Software and firmware lifecycle issues
                        	EOL/legacy systems
                        	Supply chain vulnerabilities
        •	🔐 Authentication & Authorization Basics
                o	Authentication types
                        	Single-factor, Two-factor, MFA
                        	Something you know/have/are
                        	Passwords, OTPs, Smart cards, Biometrics
                o	Credential Storage Principles
                        	Hashing vs Encryption
                        	Salted hashes (bcrypt, scrypt)
                        	Insecure storage examples (plain text, reversible encryption)
                o	Authorization Models
                        	RBAC, ABAC, DAC, MAC
                        	Access Control Lists (ACLs)
                        	Principle of least privilege
                        	Segregation of duties
        •	🔒 Encryption Fundamentals
                o	Symmetric vs Asymmetric Encryption
                o	Common algorithms: AES, RSA, ECC
                o	Hashing algorithms: SHA family, MD5 (deprecated)
                o	Encoding vs Encryption vs Hashing
                o	SSL/TLS basics (how HTTPS works)
                o	Certificates and PKI
                        	Root, intermediate, leaf certs
                        	Certificate validation and revocation (CRL/OCSP)
        •	📊 Security Policies & Compliance
                o	What are security policies?
                        	Acceptable Use Policy
                        	Password Policy
                        	Data Retention Policy
                        	Remote Work Policy
                o	Introduction to compliance
                        	ISO 27001
                        	NIST 800-series
                        	SOC 2
                        	GDPR overview (personal data, consent, DSRs)
                        	HIPAA overview
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
                        	Phishing recognition
                        	Social engineering prevention
                        	Data classification and handling
📁 Filesystems & Storage
        •	💾 Filesystem Concepts
                o	What is a filesystem?
                        	Purpose and role in OS
                        	Relation to physical storage
                o	Structure of a filesystem
                        	Blocks, clusters, sectors
                        	Inodes (Unix/Linux)
                        	MFT (Windows NTFS)
                o	File types and metadata
                        	Regular files, directories, symbolic links
                        	Permissions and timestamps
                        	Hidden/system attributes
        •	🧷 Common Filesystems
                o	FAT32
                        	Legacy use cases
                        	Max file/partition size
                        	Lack of permissions
                o	NTFS
                        	Journaling
                        	ACL-based permissions
                        	Alternate data streams (ADS)
                        	Encryption (EFS)
                o	exFAT
                        	Use in USB and SD cards
                        	Compatibility
                o	ext2/ext3/ext4
                        	Differences in journaling
                        	Use of inodes
                        	Linux compatibility
                o	Btrfs, XFS, ZFS (overview)
        •	🧩 Storage Technologies
                o	HDD vs SSD
                        	Mechanical vs flash memory
                        	Lifespan, wear leveling
                o	Hybrid drives (SSHD)
                o	NVMe & SATA interfaces
                o	Storage controllers (RAID overview)
                        	RAID levels: 0, 1, 5, 6, 10
                        	Software vs Hardware RAID
        •	🗂️ Mounting & Partitioning
                o	Partition tables
                        	MBR vs GPT
                        	Primary vs extended partitions
                o	Mounting concepts
                        	Mount points
                        	Fstab (Linux)
                        	Disk Management (Windows)
                o	Formatting and initialization
                        	Quick format vs full format
                        	Filesystem check (chkdsk, fsck)
        •	🧪 Practical Tools & Utilities
                o	Windows
                        	Disk Management GUI
                        	diskpart, format, chkdsk, fsutil
                        	BitLocker (intro only)
                o	Linux
                        	lsblk, fdisk, parted, mkfs, mount, umount
                        	df, du, fsck, tune2fs, blkid
        •	🔐 Security & Forensics Aspects
                o	Deleted file recovery
                        	File carving basics
                o	Journaling and write logs
                        	Use in incident investigation
                o	Hidden data and steganography
                o	Access control implications
                        	Permissions on file-level
                        	Filesystem encryption

🧩 Virtualization & Containers
        •	🧰 Virtualization Basics
                o	What is virtualization?
                        	Concept of abstraction
                        	Benefits: isolation, scalability, testing environments
                o	Hypervisors
                        	Type 1 (bare-metal) vs Type 2 (hosted)
                        	Examples: VMware ESXi, Microsoft Hyper-V, VirtualBox
                o	Guest OS vs Host OS
        •	🖥️ Working with Virtual Machines
                o	Creating VMs
                        	ISO selection and installation
                        	Assigning virtual hardware: CPU, RAM, disk, network
                o	Snapshots and cloning
                        	Use cases for testing and recovery
                o	VM networking modes
                        	NAT, bridged, host-only
        •	🧱 Containers Fundamentals
                o	What are containers?
                        	Difference from VMs
                        	Use of shared OS kernel
                o	Container engines
                        	Docker: image, container, volume, network
                        	Podman (rootless alternative)
                o	Dockerfile basics
                        	Image layering, build process
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
                        	VirtualBox, VMware Workstation
                        	QEMU, KVM
                o	Containers
                        	Docker CLI
                        	Docker Desktop GUI
                        	docker inspect, docker exec, docker logs
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
                        	Creating bulk users and groups
                        	Enforcing password policies
                        	Querying trust relationships
                        	Searching nested groups
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
