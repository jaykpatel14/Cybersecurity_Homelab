# 🏠 Cybersecurity HomeLab Setup

## 📌 Overview
This repository documents my **Cybersecurity HomeLab** for **penetration testing, security monitoring, and incident response**. The goal is to **simulate real-world attacks, detect them, and improve defensive measures**.

### 📍 **Network Architecture Diagram**
![alt text](<Untitled Diagram.drawio.png>)

## 🚀 **Lab Components**
| **Component**       | **Purpose** |
|---------------------|-------------|
| 🛡️ **Firewall (pfSense)** | Protects network & segments traffic between LAN, DMZ, and attacker machine |
| 🎯 **Metasploitable 2 (DMZ)** | Vulnerable machine used for **penetration testing** |
| 🔍 **Splunk (SIEM - Ubuntu Server)** | Log collection & analysis for **attack detection** |
| 💾 **Active Directory (Windows Server)** | Centralized authentication for Windows 10 machines |
| 🖥️ **Windows 10 (Domain-Joined)** | Workstation used for **attack simulations** |
| 🏴‍☠️ **Kali Linux (Attacker Machine)** | Offensive security tools for **network scanning & exploitation** |

---

## 🔥 **Current Progress**
✅ **Configured:**
- [x] Active Directory (Windows Server)
- [x] Windows 10 (Domain-Joined)
- [x] Splunk SIEM on Ubuntu Server
- [x] Metasploitable 2 (Vulnerable Machine)
- [x] pfSense Firewall for Network Segmentation
- [x] Kali Linux for Attacks

🔜 **Next Steps:**
- [ ] Configure **Windows Event Forwarding to Splunk**
- [ ] Perform **Attacks from Kali (Pass-the-Hash, Kerberoasting)**
- [ ] Implement **Detection Rules in Splunk**
- [ ] Set up **Snort/Suricata IDS for Network Threats**
- [ ] Document **SIEM Dashboards & Alerts**

---

## 🛠️ **Tools & Technologies Used**
- **Windows Server & Active Directory**
- **Splunk (SIEM)**
- **pfSense Firewall**
- **Metasploit Framework**
- **Wireshark & Nmap**
- **Sysmon for Windows Event Logging**
- **Suricata/Snort for IDS/IPS**

---

## 📖 **Attack & Detection Scenarios**
### 🔴 **Planned Attacks**
✅ **Reconnaissance:** Nmap & SMB Scanning  
✅ **Exploitation:** Pass-the-Hash, LLMNR Poisoning  
✅ **Privilege Escalation:** Kerberoasting, Mimikatz  
✅ **Persistence & Lateral Movement:** PsExec, RDP Exploitation  

### 🟢 **Planned Detection**
🔹 **Splunk Alerts:** Unusual login attempts, PowerShell executions  
🔹 **Sysmon Logs:** Process injection, Credential dumping  
🔹 **Firewall Rules:** Blocking unauthorized traffic  

---

## 📂 **How to Use This Repo**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/homelab-setup.git
