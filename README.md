Splunk SIEM Setup on Ubuntu

🛠 Project Overview

This project involves setting up Splunk Enterprise on an Ubuntu machine to collect, analyze, and visualize security logs. Splunk is widely used in cybersecurity for Security Information and Event Management (SIEM), log monitoring, and incident detection.

⚙️ Technology Used

Ubuntu 22.04 (Server/Desktop)

Splunk Enterprise (Free Version)

Linux Terminal (Command Line Interface)

📌 Installation Steps

Step 1: Download Splunk

Open a terminal and download Splunk using wget:

wget -O splunk-ubuntu.deb https://download.splunk.com/products/splunk/releases/latest/linux/splunk-latest-linux-2.0-amd64.deb

Once downloaded, install Splunk:

sudo dpkg -i splunk-ubuntu.deb

Step 2: Enable Splunk as a Service

Move to the Splunk installation directory:

cd /opt/splunk/bin

Accept the license agreement and enable Splunk at boot:

sudo ./splunk enable boot-start --accept-license

Start Splunk:

sudo ./splunk start

You will be prompted to set up an admin username and password.

Step 3: Access Splunk Web Interface

Open a web browser and go to:

http://<your-server-ip>:8000

Log in with the admin credentials created earlier.

📷 Screenshots

Below is a screenshot of the successful Splunk Web UI setup:

🎯 Key Learnings

Hands-on experience with SIEM tools.

Log collection and analysis for cybersecurity monitoring.

Splunk service configuration on Linux.
