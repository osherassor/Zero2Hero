# 🪠 Windows Internals

## 🔧 Windows Architecture Overview
- Kernel mode vs User mode
- Executive, HAL, Kernel, Subsystems
- Native APIs vs Win32 APIs
- Object Manager
- Registry subsystem
- Environment subsystems (e.g., POSIX, WoW64)
- Windows Session and Window Station concepts

## 🔢 Filesystems and Storage
- NTFS vs FAT32 vs exFAT
- Alternate Data Streams (ADS)
- Cluster sizes, MFT, journaling
- Symbolic links and junction points
- Encryption (EFS)
- Disk Quotas
- Volume Shadow Copy Service (VSS)
- Diskpart, Mountvol, Disk Management
- BitLocker fundamentals

## 📁 Windows Registry
- Registry structure: Hives, Keys, Values
- Important hives: HKLM, HKCU, HKCR, HKU, HKCC
- Boot time configuration
- Autostart locations
- Registry permissions and auditing
- REG files and automation
- Using reg.exe, regedit, PowerShell
- Malware persistence in registry
- Virtualized registry for UWP and WoW64

## 🌐 User and Permission Management
- User types: local, domain, system
- NTLM and Kerberos overview
- User Account Control (UAC)
- SIDs and RIDs
- ACLs, ACEs, DACL, SACL
- Effective permissions calculation
- Security principals and tokens
- Using icacls, whoami, takeown
- Integrity levels and AppContainer

## ⚖️ Services and Scheduled Tasks
- Service Control Manager (SCM)
- services.msc and sc.exe
- Creating and configuring services
- Service permissions and SDDL strings
- Service start types
- Scheduled Tasks via Task Scheduler
- Event-based triggers
- Task XML configuration files
- Persistence and privilege escalation vectors
- Monitoring scheduled tasks

## 🤜 PowerShell Internals
- Cmdlets vs functions vs scripts
- Execution policies
- PowerShell profiles and persistence
- Modules and importing
- Objects and pipelines
- Remoting and Invoke-Command
- Logging and transcription
- Using PowerShell to manage system settings
- Security features (Constrained Language Mode)
- PS logging (event IDs, transcripts)

## 🔄 Process, Thread & Memory Management
- Processes, threads, handles, jobs
- Process Explorer & Process Monitor tools
- DLL injection and reflective DLLs
- Memory regions: heap, stack, image
- Virtual memory and paging
- Working set, commit charge
- Handle tables and leaks
- Windows Internals tools (VMMap, RAMMap)
- Debugging symbols (PDBs)
- Crash dump analysis

## 🌌 Boot Process & Startup
- BIOS vs UEFI
- Secure Boot
- Boot Configuration Data (BCD)
- Bootmgr, winload, winresume
- Safe mode, recovery environment
- Boot logs and troubleshooting
- Autostart locations (registry, startup folders)
- Startup Repair, MSConfig

## 🔎 Logging and Event Tracing
- Event Viewer overview
- Windows event log types
- Event log locations (evtx)
- Important security and system event IDs
- Custom views and filters
- Forwarded events
- ETW (Event Tracing for Windows)
- Sysmon basics
- Log archiving and retention

## 🛡️ Windows Security Features
- Windows Defender architecture
- SmartScreen
- Controlled Folder Access
- Credential Guard
- Device Guard
- Windows Firewall and advanced rules
- AppLocker and WDAC
- Security baselines
- LSA protection

## ⌛ Command Line Fundamentals (CMD)
- Overview of cmd.exe
- Command interpreter vs scripting engine
- Internal vs external commands
- Command chaining (&&, ||, &)
- Command history and navigation
- Variables and environment variables
- Redirection (>, >>, <) and piping (|)
- Wildcards and globbing (*, ?)
- Using help and /? syntax

### ✍️ File & Folder Operations
- dir, cd, mkdir, rmdir, del, copy, move, xcopy, robocopy
- Attributes: attrib, icacls
- tree, fsutil
- Hidden/system files
- Recursive deletion

### ⚙️ System Information & Configuration
- systeminfo, hostname, ver, set, setx
- tasklist, taskkill
- wmic basics
- ipconfig, netstat, ping, tracert
- net use, net view, net session
- assoc, ftype

### ⏱ Scheduling & Automation
- Creating batch files (.bat)
- Using schtasks to create scheduled tasks
- Startup folder scripts
- call, goto, pause, choice, if, for, setlocal
- Comments and script headers

### 🌐 Networking Commands
- ping, tracert, pathping
- netsh basics
- ipconfig /all
- arp, nbtstat, route print, netstat -ano
- telnet and ftp
- DNS lookups with nslookup

### ⚖️ User and Access Management
- net user, net localgroup, net group
- whoami, runas, echo %username%
- cacls, icacls, takeown
- Modifying ownership and permissions

### 🛠️ Troubleshooting and Diagnostics
- Reading logs with wevtutil
- sfc /scannow, chkdsk, DISM
- echo, pause, cls, color
- Testing scripts safely
- Interacting with .reg files

## 📁 File Types and Structures
- Executable formats: .exe, .dll, .sys, .bat, .ps1
- Document formats: .docx, .pdf, .rtf, .txt
- Archive formats: .zip, .rar, .7z, .tar.gz
- Image formats: .jpg, .png, .bmp, .svg
- Multimedia formats: .mp4, .mp3, .avi, .mkv
- Configuration formats: .ini, .conf, .yaml, .json, .xml
- Log files: structure, delimiters, timestamps, and severity levels
- Proprietary vs Open formats

## 🧮 Encoding and Character Sets
- ASCII and Extended ASCII
- Unicode: UTF-8, UTF-16, UTF-32
- Base64 encoding and decoding
- URL encoding
- Hexadecimal and Binary representations
- Endianness (Big-endian vs Little-endian)
- BOM (Byte Order Mark) and its impact on file parsing

## 🧪 Parsing and Manipulation Tools
- cat, less, more, head, tail, strings
- xxd, hexdump, binwalk, file
- jq, xmlstarlet, yq, csvkit
- iconv and character encoding conversion

## 🔎 File Metadata & Attributes
- File timestamps: Created, Modified, Accessed
- File permissions and ACLs
- Alternate Data Streams (ADS) on NTFS
- Hidden/system attributes
- Signature validation and hash comparison (MD5, SHA1, SHA256)

## 📦 Forensics Considerations
- Understanding file carving
- Recognizing anomalies in file headers/footers
- Common obfuscation techniques in documents (e.g., macros)
- File magic numbers
