# 🔄 Reverse Engineering Fundamentals

## 🎯 Purpose & Goals
- Understand how software works without access to the source code  
- Analyze compiled applications, malware, or unknown binaries  
- Identify vulnerabilities, hidden features, and logic flaws  

---

## 🛠 Tools & Setup
- Disassemblers [Ghidra](httpsghidra-sre.org), [IDA Pro](httpshex-rays.comida-pro), [Binary Ninja](httpsbinary.ninja)  
- Debuggers [x64dbg](httpsx64dbg.com), [WinDbg](httpslearn.microsoft.comen-uswindows-hardwaredriversdebugger), [OllyDbg](httpwww.ollydbg.de)  
- Scripting tools [Frida](httpsfrida.re), [Radare2](httpsrada.ren), [Angr](httpsangr.io)  
- Execution environments Isolated WindowsLinux VMs with snapshots  
- File analysis [PEStudio](httpswww.winitor.com), [CFF Explorer](httpsntcore.compage_id=388), `readelf`, `objdump`  

---

## 🧱 Binary Formats
- Common executable formats PE (Windows), ELF (Linux), Mach-O (macOS)  
- Understanding headers, sections, imports, and exports  
- Static linking vs dynamic linking  

---

## ⚙️ Assembly Language Basics
- Key concepts Registers (EAX, ECX, etc.), Stack, Instruction Pointer (EIP)  
- Common instructions `MOV`, `PUSH`, `POP`, `CALL`, `RET`, `JMP`  
- Calling conventions `cdecl`, `stdcall`, `fastcall`  
- Recognizing function prologues and epilogues  

---

## 🧠 Control Flow Analysis
- Analyzing function trees and call graphs  
- Understanding loops, branches, and conditionals  
- Identifying control flow obfuscation and techniques to simplify it  

---

## 🐞 Debugging & Dynamic Analysis
- Setting breakpoints and tracing execution  
- Inspecting memory heap, stack, and registers  
- Identifying anti-debugging tricks and bypassing them  

---

## 🛡 Anti-Reversing Protections
- Identifying packers and code obfuscation  
- Recognizing virtualized code and custom VM architectures  
- Detecting and analyzing self-modifying code  

---

## 🧪 Malware Reverse Engineering
- Behavior analysis in sandboxed environments  
- Capturing and analyzing network traffic  
- Extracting Indicators of Compromise (IOCs)  
- Comparing signature-based vs behavioral detection  

---

## 🔐 Cryptographic Analysis
- Recognizing cryptographic primitives (e.g., AES, RSA, SHA)  
- Analyzing key handling, generation, and storage  
- Detecting custom or weak crypto implementations  

---

## 🧾 Deliverables
- Annotated disassembly and pseudocode  
- Behavioral and functional summaries  
- IOCs for threat intelligence  
- Reverse engineering technical report  
- Risk assessment and remediation recommendations  
