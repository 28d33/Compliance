# 🛡️ Compliance Assessment – Fed F1rst Control Systems

A strategic cybersecurity and compliance assessment project focused on securing Windows, macOS, and Linux environments, enforcing enterprise security policies, and ensuring cloud infrastructure is audit-ready and aligned with industry standards.

---

## 🧭 Project Overview

**Client:** Fed F1rst Control Systems  
**Domain:** Government Technology & Infrastructure  
**Goal:** Strengthen the compliance posture across hybrid environments (Windows, macOS, Linux, Cloud) while aligning with cybersecurity standards such as CMMC, HIPAA, and ISO 27001.

---

## 🔐 Section 1: System Hardening Strategy

### ✅ Windows 10 Hardening Checklist
- Enable automatic updates
- Enforce strong password policies
- Enable Windows Defender Antivirus
- Configure firewalls (public/private)
- Rename/disable admin accounts
- Enable BitLocker Drive Encryption

### 🍎 macOS Hardening Checklist
- Enable FileVault for full disk encryption
- Use MDM for centralized policy management
- Disable guest access & auto-login
- Enforce secure login (strong passwords, recovery keys)
- Enable system firewall and restrict incoming connections
- Enable automatic OS/app updates

---

## 📜 Section 2: Security Policies

### 📧 Email Security Policy
- Use corporate email accounts only
- Enforce encryption for sensitive data
- Prohibit suspicious attachment and link access
- Use strong, unique passwords
- Report phishing via designated process

### 📱 BYOD Policy
- Enroll in company-approved MDM
- Enforce encryption: FileVault (macOS), BitLocker (Windows), Full-Disk (Android)
- Restrict use to company-approved apps
- Enforce biometric/password authentication
- Prohibit rooted/jailbroken devices
- Enable remote wipe on compromised devices

---

## 📊 Section 3: Self Assessment Summary

### 🪟 Windows 10 Compliance (Partial Highlights)
| Control | Status |
|--------|--------|
| Built-in Admin Account Disabled | ✅ Met |
| Firewall Enabled | ✅ Met |
| Strong Passwords | ❌ Not Met |
| USB Port Restrictions | ❌ Not Met |
| Audit Logging Enabled | ❌ Not Met |

**Remediation Plan:**
- Enforce strong passwords via Group Policy
- Enable advanced audit policies and logging
- Restrict USB via device ID whitelisting

### 🐧 Linux Compliance (Ubuntu 24.04)
| Control | Status |
|--------|--------|
| Current Security Updates | ✅ Met |
| /var Separate Partition | ❌ Not Met |
| Disable Automount | ❌ Not Met |
| AIDE Installed | ❌ Not Met |
| Disable Unused Services (tftp, ftp, DHCP) | ✅ Met |
| CUPS/Automount Disabled | ❌ Not Met |
| Audit Log Management | ❌ Not Met |

**Recommendations:**
- Create a separate `/var` partition
- Install and configure AIDE
- Set audit log size and retention
- Harden services and daemon settings

---

## ☁️ Section 4: Cloud Configuration & Monitoring

### 🧱 Windows Server Build Sheet
- **OS Version:** Windows Server 2022 Datacenter
- **Firewall Rules:** Allow only HTTP(S), restrict RDP
- **IIS Installation:** Configure with secure defaults
- **Admin Hardening:** Rename default account
- **Logging:** Enable event forwarding + Azure Monitor
- **Patch Management:** Use Azure Update or WSUS

### 🛡️ Enhancing Security with CASB
- **Visibility:** Detect Shadow IT usage
- **DLP Enforcement:** Prevent sensitive data exposure
- **Threat Detection:** Behavior analytics and anomaly detection
- **Access Control:** Conditional access by device, location, user role
- **Compliance Reporting:** Automated logs, regulatory dashboards

---

## 🧰 Tools Used

- **PowerShell** – Windows compliance scripting
- **AuditD / AIDE** – Linux auditing and integrity
- **MDM (Jamf, Intune)** – Device compliance enforcement
- **CASB (Microsoft Defender for Cloud Apps, Netskope)** – Cloud access control
- **Azure Security Center / Monitor** – Server hardening and logging

---

## ✍️ Author

**Deekshith A**  
Cybersecurity Analyst | Compliance Engineer | Cloud Security Specialist

---

## 📄 License

This project is intended for educational, training, and compliance reference purposes only.
