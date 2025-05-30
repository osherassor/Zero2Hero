## ☁️ Cloud Penetration Testing

### ☁️ Goals & Objectives
- Simulate attacks targeting cloud infrastructure and services  
- Identify misconfigurations, weak IAM policies, and exploitable cloud components  
- Evaluate security posture across SaaS, PaaS, and IaaS models  
- Provide actionable remediation guidance  

### 🔧 Environment Setup & Access
- Target cloud providers: AWS, Azure, GCP  
- Create test environments with various services (VMs, containers, storage, databases)  
- Set up credentials with different roles (admin, user, developer)  
- Define rules of engagement and scope  

### 🔍 Reconnaissance & Enumeration
- DNS enumeration for cloud domains and subdomains  
- Identifying services: S3 buckets, Azure Blobs, Google Storage  
- Passive recon using OSINT (e.g., GitHub, Google dorks, crt.sh)  
- Tools: Amass, Subfinder, CloudEnum, S3Scanner  

### 🛡 IAM Misconfiguration Testing
- Identify overprivileged roles and users  
- Misconfigured policies and permission boundaries  
- Exploiting AssumeRole and trust relationships  
- Enumeration with tools: ScoutSuite, PMapper, IAM Vulnerable Policies  
- Privilege escalation paths (e.g., attaching policies, lambda abuse)  

### 🔓 Public Cloud Storage & Database Exposure
- Check for publicly accessible S3, Azure Blobs, and GCP Buckets  
- Enumeration of misconfigured DBs (MongoDB, Elasticsearch, Redis)  
- Data extraction and access testing  

### ⚙️ Service-Specific Exploitation

#### AWS
- Lambda privilege escalation  
- SSRF on EC2 metadata  
- Misused IAM roles and STS  
- Secrets Manager and Parameter Store leaks  

#### Azure
- Azure AD abuse (e.g., password spray, token replay)  
- Exploiting Azure Functions and App Services  
- Azure Automation Runbooks  

#### GCP
- IAM misconfiguration and privilege escalation  
- Exploiting Cloud Functions & metadata  
- Service account impersonation  

### 🛠 Containers in Cloud
- EKS, AKS, GKE cluster enumeration and exploitation  
- Exposed dashboards (e.g., Kubernetes, Portainer)  
- Container breakout techniques  
- Misconfigured container roles and secrets  

### 🔍 Logging, Monitoring & Detection Evasion
- Analyze logging capabilities: AWS CloudTrail, Azure Monitor, GCP Cloud Logging  
- Evade detection using obfuscation, proxychains, minimal privileges  
- Detection of honeypots and decoys  

### 🧩 Post-Exploitation & Lateral Movement
- Enumerate cross-service relationships  
- Use harvested credentials to access new targets  
- Pivoting through serverless functions or identity impersonation  

### 📦 Deliverables
- Executive summary with risk ratings  
- Technical findings with reproduction steps and screenshots  
- Cloud architecture diagram with findings highlighted  
- IAM and privilege graphs (e.g., PMapper)  
- Remediation steps and cloud-specific hardening advice  
- MITRE ATT&CK mapping for cloud-based techniques  

---

📌 **MITRE ATT&CK Matrix (Cloud)**  
Explore the full MITRE ATT&CK for cloud techniques here:  
🔗 https://attack.mitre.org/matrices/enterprise/cloud/
