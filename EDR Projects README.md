# 🖥️ Endpoint Threat Detection and Response Using Wazuh

## 📌 Project Overview

This project demonstrates how to set up and use **Wazuh**, a powerful open-source SIEM tool, for detecting and responding to endpoint-based cyber threats. Simulated attacks such as brute-force login attempts, port scans, and reverse shell execution were performed on a monitored Linux environment. Using **custom rules**, real-time alerts, and centralized logging, this project shows how Wazuh supports Security Operations Center (SOC) functions like threat hunting, compliance, and active response.

---

## 🎯 Objectives

- 🛠️ Deploy Wazuh Manager, Indexer, Dashboard on Ubuntu
- 🔗 Connect Kali Linux as an endpoint agent
- 🔍 Simulate cyberattacks: failed SSH logins, scans, reverse shells
- 📈 Visualize alerts and logs using Wazuh’s web dashboard
- ⚙️ Customize rules for better detection and automated responses

---

## 🛠️ Tools & Technologies Used

| 🔧 Tool          | 📝 Purpose                                |
|------------------|--------------------------------------------|
| 🧠 Wazuh Manager  | SIEM engine for analysis and log collection |
| 🔍 Wazuh Agent    | Installed on endpoint (Kali Linux)         |
| 🖥️ Ubuntu 22.04   | Host for Wazuh Manager                     |
| 🐍 Kali Linux     | Simulated attacker/endpoint                |

---

## 🧱 Setup Summary

1. 🧰 Install Wazuh Stack (Manager + Dashboard + Indexer) on Ubuntu:

🌐 Access Dashboard at https://<ubuntu-ip>:443

➕ Add Kali Linux as Agent:

Copy agent registration script from Dashboard

Run on Kali:

bash
Copy
Edit
sudo systemctl enable wazuh-agent
sudo systemctl start wazuh-agent
✅ Agent becomes active and starts sending logs to Wazuh

🚨 Attack Simulations & Detection
🛡️ Attack Type	✅ Detection by Wazuh
❌ SSH Brute-force	Alert via authentication logs
📡 Nmap Port Scan	Detected via scan signatures
🔁 Reverse Shell	Flagged via command pattern rules
💾 Malware File Drop	Detected by File Integrity Monitoring (FIM)

🔍 Key Wazuh Modules Used
📊 Dashboard – Real-time view of agents, alerts, severity

🧠 Threat Hunting – Manual investigation of log data

📌 MITRE ATT&CK – Map alerts to attacker tactics

🛠️ File Integrity Monitoring (FIM) – Track file changes

🔐 Vulnerability Detection – Identify weak or outdated software

🔧 Rule Customization – Add new detection logic via XML rules

⚡ Active Response – Automatically block or respond to threats

🧠 Key Learning Outcomes
💡 Real-world use of Wazuh in endpoint monitoring

🔄 Integration of agents and central log analysis

📑 Custom rule creation for fine-tuned detection

🎯 Enhanced visibility into Linux endpoint behavior

🧰 SOC-level threat detection using open-source tools

## Full Report

📎 Full Project Report

[📄 Click here to view the full PDF report](https://drive.google.com/file/d/1WYikq51VfyXrMzTdne4ZAFixrSfCymWi/view?usp=sharing)
