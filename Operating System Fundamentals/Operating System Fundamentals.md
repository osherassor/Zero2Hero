# 🖥️ Operating System Fundamentals

## 🧱 What is an Operating System?
- Define OS as a mediator between hardware and applications
- Key responsibilities: resource management, UI, hardware abstraction
- History: batch processing → time sharing → graphical OS
- Real-time vs general-purpose OS
- Embedded vs desktop vs server OS
- Monolithic vs microkernel design
- Overview of major OS families (Windows, UNIX/Linux, macOS)
- Multitasking, multiprocessing, multiuser capabilities
- Kernel space vs user space
- OS boot sequence (generic model)

## 🧠 Core OS Components
- Kernel: role and sub-components
- Process Scheduler: algorithms and priorities
- Memory Manager: virtual memory, paging
- File System Manager
- Device Drivers and Hardware Abstraction Layer (HAL)
- System Calls and APIs
- User Interface: CLI vs GUI
- Daemons/Services background processes
- Interprocess Communication (IPC) models
- Module loading and kernel extensions

## 🧮 Process Management
- What is a process?
- States: Ready, Running, Waiting, Terminated
- Process Control Block (PCB)
- Threads: multithreading, thread pools
- Scheduling strategies: FIFO, Round-Robin, Multilevel Queue
- Context switching
- Foreground vs background processes
- Process hierarchy and parent-child relationships
- Resource allocation per process
- Orphan and zombie processes

## 🧬 Memory Management
- Address spaces: logical vs physical
- Paging, segmentation
- Page tables and TLBs (Translation Lookaside Buffers)
- Virtual memory and swap
- Memory fragmentation
- Allocation techniques: First Fit, Best Fit, Buddy System
- Memory protection and isolation
- Demand paging and page faults
- Heap vs stack memory regions
- Shared memory models

## 📁 File System Management
- File attributes: metadata, permissions, timestamps
- File types and extensions
- Directory structures: single-level, tree, acyclic graphs
- Mounting and partitions
- File system journaling
- File locks and access controls
- Inodes and data blocks (in Linux)
- FAT table structure (Windows)
- Symbolic and hard links
- File compression and encryption

## 🔌 Input/Output & Device Management
- I/O device categories: character vs block
- Device drivers and driver stacks
- Interrupts and polling mechanisms
- Plug-and-play architecture
- Buffering and spooling
- DMA (Direct Memory Access)
- I/O scheduling
- USB stack, PCI management
- Driver signing and trust chains
- Hot-swapping devices

## 🔒 User & Access Control
- Authentication: local, federated, biometric
- Authorization: DAC, MAC, RBAC
- Session control and isolation
- Access tokens and privileges
- User roles and permission groups
- Credential storage mechanisms
- Principle of least privilege
- Security identifiers and ACLs
- Login types: console, remote, SSH, RDP
- User namespaces (Linux container model)

## 🔁 Multitasking, Multithreading, Multiprocessing
- Differences and use-cases
- CPU affinity and thread pinning
- Thread vs process isolation
- Kernel-mode vs user-mode threading
- Preemptive vs cooperative multitasking
- Symmetric multiprocessing (SMP) and scheduling
- Hyper-threading awareness
- Locks, semaphores, and race conditions
- Thread synchronization issues
- Deadlocks and starvation

## 📡 Networking Basics in OS
- OSI layer integration into system stack
- NIC drivers and interface configuration
- Sockets and port binding
- TCP/IP stack and loopback interfaces
- Network configuration files
- Firewalls and packet filters
- Connection management and timeouts
- DNS resolver settings
- DHCP client configuration
- ICMP error handling

## 🧰 System Configuration & Maintenance
- System logs and log rotation
- Configuration file hierarchy
- Scheduled jobs (cron, task scheduler)
- Time sync (NTP, system clock)
- Locale and language settings
- System updates and patching
- Bootloader configuration
- Init systems (init, systemd, launchd)
- Emergency and recovery modes
- Snapshot and rollback mechanisms
