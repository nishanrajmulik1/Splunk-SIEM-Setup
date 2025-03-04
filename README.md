# Splunk SIEM Setup on Ubuntu 🚀

## 📌 Project Overview
This project demonstrates the installation and setup of **Splunk Enterprise** on an **Ubuntu 22.04** machine for **Security Information and Event Management (SIEM)**, log monitoring, and incident detection.

## 🛠 Technology Stack
- **Operating System:** Ubuntu 22.04 (Server/Desktop)
- **SIEM Tool:** Splunk Enterprise (Free Version)
- **Command Line Interface:** Linux Terminal

---

## 📥 Installation Steps

### **Step 1: Download Splunk**
Open a terminal and download Splunk using `wget`:

```bash
wget -O splunk-ubuntu.deb https://download.splunk.com/products/splunk/releases/latest/linux/splunk-latest-linux-2.0-amd64.deb
```
Once downloaded, install Splunk:
```bash
sudo dpkg -i splunk-ubuntu.deb
```

Step 2: Enable Splunk as a Service
Move to the Splunk installation directory:
```bash
cd /opt/splunk/bin
```
Accept the license agreement and enable Splunk at boot:
```bash
sudo ./splunk enable boot-start --accept-license
```
Start Splunk:
```bash
sudo ./splunk start
```

Step 3: Access Splunk Web Interface
Once Splunk is running, open a web browser and navigate to:
```bash
http://10.0.0.130:8000
```

📸 Screenshots
![Splunk](screenshots/Splunk Webdashboard.png) 

🎯 Key Learnings
Hands-on experience with Splunk SIEM for security monitoring.
Understanding log collection and analysis in cybersecurity.
Configuring and managing Splunk services on Linux.
