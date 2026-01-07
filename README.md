# 🛡️ Multi-Platform Penetration Testing Lab
### Real-world exploitation of Linux & Windows vulnerabilities

---

## 📖 Overview

This repository contains a **hands-on penetration testing lab** that demonstrates how real-world vulnerabilities can be identified, exploited, and analyzed across multiple operating systems. The project focuses on **kernel privilege escalation, web application attacks, and Windows remote code execution**, using real CVEs and industry-standard security tools.

This lab showcases practical offensive security skills, structured testing methodology, and security impact analysis.

---

## ❗ Problem Statement

Many organizations continue to operate:
- Outdated operating systems
- Unpatched kernels
- Legacy services with known vulnerabilities

These weaknesses make systems easy targets for attackers and frequently lead to **full system compromise**.

---

## 🚨 Why This Matters

Failure to patch known vulnerabilities can result in:
- Root / SYSTEM-level access
- Data breaches and credential theft
- Lateral movement within networks
- Compliance failures and financial loss

This project demonstrates how **small security gaps can lead to complete compromise**.

---

## 🧠 Solution Overview

The lab consists of **three intentionally vulnerable virtual machines**:

- **Ubuntu 20.04 LTS**
- **Debian 8 (Jessie)**
- **Windows 7 SP1**

Each machine is tested using a structured penetration testing workflow:
1. Enumeration
2. Vulnerability identification (CVE mapping)
3. Exploitation
4. Privilege escalation
5. Impact analysis

---

## 🏗️ Architecture / Workflow

Attacker (Kali Linux)
↓
Network Scanning & Enumeration
↓
Vulnerability Identification (CVEs)
↓
Exploit Execution
↓
Privilege Escalation
↓
Root / SYSTEM Access


---

## 🧰 Tech Stack & Tools

### Operating Systems
- Ubuntu 20.04 LTS
- Debian 8 (Jessie)
- Windows 7 SP1

### Tools & Frameworks
- Metasploit Framework
- Nmap
- Netcat
- Custom exploit scripts
- Linux kernel exploits (Dirty Pipe, Dirty COW)

---

## ✨ Key Features

- Real CVE-based exploitation
- Linux and Windows attack scenarios
- Kernel-level privilege escalation
- SMB remote code execution
- Web application XSS exploitation
- Detailed vulnerability documentation

---

## ▶️ Running the Lab Locally

> ⚠️ **For educational use only. Run in an isolated lab environment.**

### Prerequisites
- VirtualBox or VMware
- Kali Linux attacker VM
- Vulnerable target VMs
- Host-only or internal network configuration

### Setup

```bash
sudo apt update && sudo apt upgrade -y
msfconsole


Ensure all virtual machines are on the same network before exploitation.

🧪 Example Exploits
EternalBlue (Windows 7)
use exploit/windows/smb/ms17_010_eternalblue
set RHOSTS <target_ip>
exploit

Dirty COW (Linux Privilege Escalation)
gcc dirtycow.c -o dirtycow
./dirtycow



⚠️ Limitations

Focuses on known vulnerabilities only

No automated patching or remediation

No Active Directory environment

🚀 Future Enhancements

Active Directory attack scenarios

Detection and logging (SIEM integration)

Automated vulnerability scanning

Container-based vulnerable environments

📚 What I Learned

Practical exploitation of real-world vulnerabilities

Kernel-level privilege escalation techniques

Windows SMB exploitation

Importance of patch management

Professional penetration testing documentation

⚖️ Disclaimer

This project is for educational and ethical purposes only.
Do not test systems without explicit authorization.
