# 📊 Splunk SIEM Setup

## 📌 Project Overview

This project documents the step-by-step setup of a **Splunk-based Security Information and Event Management (SIEM)** lab environment to monitor and analyze logs from Windows endpoints.

The goal is to simulate real-world attack scenarios, forward logs to Splunk, and create meaningful detections using built-in apps and custom searches. This project demonstrates key blue team skills like log collection, correlation, alert creation, and MITRE ATT&CK mapping.

---

## 🛠️ Tools & Technologies Used

- 🧠 **Splunk Enterprise** (Free Trial)
- 💻 **Windows 10 & Server 2019** (Endpoint log sources)
- 📦 **Universal Forwarder** (for log forwarding)
- 🔍 **Sysmon** (for enriched Windows event logging)
- 🧰 **MITRE ATT&CK**
- 🖥️ **Virtualization**: VMware Workstation Pro / Proxmox

---

## 🏗️ Lab Setup Overview

| Component | Description |
|----------|-------------|
| Splunk Server | Installed on Ubuntu, acts as SIEM & analysis engine |
| Windows 10 / 2019 | Log source machines (target systems) |
| Sysmon + UF | Installed on endpoints to generate & forward logs |
| Attack Simulation | Simulated brute force, PowerShell, and malware behavior |
| Detection | Correlated logs with MITRE techniques and created alerts |

---

## 🗂️ Project Structure

```bash
Splunk-SIEM-Setup/
├── documentation/
│   └── Splunk-Install-Steps.pdf
│   └── Universal-Forwarder-Setup.md
├── dashboards/
│   └── windows-attack-detection.xml
├── searches/
│   └── powershell-abuse-search.spl
│   └── rdp-brute-force-detection.spl
├── screenshots/
│   └── splunk-dashboard.png
└── README.md
```
## 🔍 Use Cases & Example Detections

| Detection Use Case | Description | MITRE Technique |
|--------------------|-------------|------------------|
| RDP Brute Force | Multiple failed login attempts | T1110.001 |
| PowerShell Abuse | Detect encoded or suspicious scripts | T1059.001 |
| Unexpected Services | New services created by attackers | T1543.003 |

---

## ✅ What I Learned

- Installing and configuring Splunk on Linux (Ubuntu)
- Collecting and visualizing logs from Windows endpoints
- Writing detection rules and dashboards in Splunk SPL
- Mapping alerts to the MITRE ATT&CK framework

📸 Screenshots
![Splunk Dashboard](./screenshots/Splunk%20Web%20Dashboard.png)


