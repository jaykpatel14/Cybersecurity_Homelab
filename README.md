# 🏠 Cybersecurity HomeLab Setup

## 🚨 Problem Statement
Setting up a **secure and monitored IT infrastructure** is a fundamental challenge in cybersecurity. Many **SOC analysts, security engineers, and IT professionals** lack hands-on experience in configuring enterprise environments with **Active Directory, SIEM monitoring, and network security**.

This HomeLab solves this problem by:
- **Simulating a corporate IT infrastructure** with multiple virtual machines.
- **Providing an isolated, controlled environment** for testing configurations.
- **Enhancing understanding of system administration, logging, and network segmentation**.

This setup allows me to **gain practical experience in configuring and securing an enterprise-like environment** with **Windows Server, pfSense, Splunk, and Kali Linux**.

---

## 📌 HomeLab Overview
This repository documents my **Cybersecurity HomeLab**, focusing on:
- **Virtual machine setup & configuration** (VMware/VirtualBox)
- **Network segmentation & firewall rules** (pfSense)
- **Centralized authentication & access management** (Active Directory)
- **Log collection & monitoring** (Splunk)
- **System hardening & security configurations**

---

## 📍 Network Architecture
The HomeLab consists of **multiple virtual machines**, each serving a unique role in simulating an enterprise environment.

![](Untitled%20Diagram.drawio.png)

| **Component**            | **Purpose** |
|-------------------------|-------------|
| 🛡 **pfSense Firewall** | Segments traffic, protects LAN & DMZ |
| 💾 **Active Directory (Windows Server)** | Manages user authentication & domain policies |
| 🖥 **Windows 10 (Domain-Joined)** | Workstation for testing domain authentication |
| 🔍 **Splunk SIEM (Ubuntu Server)** | Log collection & system monitoring |
| 🏴‍☠️ **Kali Linux** | Used for system testing & security research |
| 💀 **Metasploitable 2** | Used as targetted machine, deployed under dmz network | 

---

✅ **Configured:**
- Virtualized environment using **VMware/VirtualBox**
- **Active Directory (Windows Server)**
- **Windows 10 (Domain-Joined)**
- **Splunk SIEM on Ubuntu Server**
- **Kali Linux setup for testing**
- **pfSense Firewall installation**
- **Metasploitable 2 installation**
- **Tested Connectivity between devices**


---

## 📂 Setup Guide
This repository includes documentation on **installing and configuring each virtual machine**:

### **1️⃣ Install Virtualization Software**
   - Download & install **VMware Workstation** or **VirtualBox**.

### **2️⃣ Set Up Virtual Machines**
   - Install **Windows Server & configure Active Directory**.
   - Install **Windows 10 & join it to the domain**.
   - Install **Splunk SIEM on Ubuntu Server**.
   - Install **pfSense Firewall & configure networking**.
   - Install **Kali Linux for testing**.
   - Install **Metasploitable 2 to demostrate dmz network**. 

### **3️⃣ Configure Network & Security Settings**
   - Assign **static IPs, subnets, and firewall rules**.
   - Enable **domain authentication & group policies**.
   - Forward **Windows event logs to Splunk**.

### **4️⃣ Validate Setup & Connectivity**
   - Test **domain authentication (Windows 10 logging into AD)**.
   - Check **pfSense firewall traffic rules**.
   - Verify **log collection in Splunk**.

📌 **For detailed instructions, check the `/docs/` folder.**

## This repository includes a /configs directory that contains all the configuration files for the HomeLab:

- Firewall Configuration
- Group Policy Objects (GPO) Settings
- Splunk Input Configuration: inputs.conf

📌 For detailed instructions, check the /config folder.

## 🛠 Tools & Technologies Used
- **VMware Workstation / VirtualBox** – Virtualization Platform
- **Windows Server & Active Directory** – User Authentication & Access Control
- **Windows 10 (Domain-Joined)** – Endpoint Testing
- **pfSense Firewall** – Network Security & Segmentation
- **Splunk SIEM (Ubuntu Server)** – Security Monitoring & Log Collection
- **Metasploitable 2** - Vulnerable machine.

---

## 📂 How to Use This Repo
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/homelab-setup.git
