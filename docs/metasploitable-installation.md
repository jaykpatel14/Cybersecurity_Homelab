# 🏴‍☠️ Installing Metasploitable 2 in VMware Workstation

## 📌 Overview
Metasploitable 2 is a **vulnerable virtual machine** designed for **penetration testing and security training**. This guide provides **step-by-step instructions** for installing Metasploitable 2 in **VMware Workstation**.

---

## **🛠️ Step 1: Download Metasploitable 2**
1. Go to the **official Rapid7 website**:  
   🔗 [Download Metasploitable 2](https://information.rapid7.com/download-metasploitable-2.html)
2. Download the **Metasploitable 2 ZIP file** for Linux.
3. Save the file to your preferred directory.

---

## **📂 Step 2: Extract the ZIP File**
1. Navigate to the folder where the ZIP file was downloaded.
2. Extract the **Metasploitable 2 archive** using your preferred tool:
   - **Windows:** Right-click → Extract All.
   - **Linux/macOS:** Use the terminal:
     ```bash
     unzip Metasploitable2-Linux.zip
     ```
3. The extracted folder will contain the **Metasploitable 2 VM files**.

---

## **💻 Step 3: Open Metasploitable 2 in VMware**
1. Open **VMware Workstation**.
2. Click **File > Open**.
3. Locate the **Metasploitable 2 folder** and open the `.vmx` file.

---

## **🔄 Step 4: Upgrade the Virtual Machine (Optional)**
1. After opening, VMware might prompt you to **upgrade the virtual machine**.
2. Click **"Upgrade this Virtual Machine"** to ensure compatibility.

---

## **🌐 Step 5: Configure Network Adapter**
1. Go to **VM > Settings**.
2. Select **Network Adapter**.
3. Change the **second network adapter** to:
   - **LAN Segment:** Set it to **DMZ** (for network segmentation).

---

## **🚀 Step 6: Start the Metasploitable 2 Machine**
1. Click **Power On this Virtual Machine**.
2. When prompted with **"Did you move or copy this virtual machine?"**, select:
   - ✅ **"I Copied It"**
3. Wait a few minutes for the system to boot.

---

## **🔑 Step 7: Login to Metasploitable 2**
1. After booting, log in using the default credentials:
   
Username: msfadmin Password: msfadmin 
