# 🔗 Active Directory & Domain Services

## 🏛️ Core Concepts of Active Directory (AD)
- What is AD and why it's used
- Centralized authentication and authorization
- Domains, trees, forests
- Logical & physical structure: DCs, OUs, Sites, Global Catalog

## 👥 Users, Groups & Access Management
- Local vs domain accounts
- Group types & scopes
- OU design and best practices
- Group nesting, RBAC, administrative tiers
- GPO basics and deep dive

## 🧠 Authentication & Trust Models
- Kerberos authentication flow (AS, TGS, TGT, ST)
- NTLMv1 vs NTLMv2
- NTLM authentication flow
- Trust relationships
- SSO and token delegation
- SID, RID, and token structure
- Pass-the-Hash (concept only, not exploitation)

## 🧰 Administrative Tools & Management

### GUI Tools
- Active Directory Users & Computers (ADUC): creating, modifying, disabling accounts
- ADAC, GPMC, ADSI Edit

### PowerShell Modules for AD
- Creating bulk users and groups
- Enforcing password policies
- Querying trust relationships
- Searching nested groups

## 🔐 Permissions, ACLs & Delegation
- NTFS permissions vs share permissions
- Effective permissions
- DACL, SACL, ACE entries
- Inheritance & blocking
- Delegation Wizard use cases
- Auditing: enabling and interpreting

## 📡 DNS Integration & SRV Records
- Role of DNS in domain joining
- SRV records for Kerberos, LDAP
- Dynamic DNS registration
- Testing DNS with `nslookup`, `nltest`

## 🧪 Diagnostics & Troubleshooting
- Common tools: `dcdiag`, `repadmin`, `nltest`, `netdom`, `whoami`
- Troubleshooting logon failures
- Diagnosing replication issues
- Reading AD event logs

## 🧬 Schema, FSMO Roles & Replication
- AD Schema explained
- Schema extensions and risks
- 5 FSMO roles and their responsibilities
- Replication flow, latency, and conflict resolution
- Site links and replication topology

## 🧩 Enterprise Design Patterns & Scenarios
- Tier 0/1/2 models
- Domain isolation vs resource forest
- Multi-domain architecture
- Trust design in mergers & hybrid clouds
- Integration with Azure AD
