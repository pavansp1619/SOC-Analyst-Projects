# 🛡️ QRadar SIEM Project: Malware Detection and Log Analysis

## 📌 Project Overview

This project simulates a real-world malware attack scenario to demonstrate how **IBM QRadar SIEM** can be used to detect, analyze, and respond to malicious activity. A **Trojan payload** was created using MSFvenom, delivered via a local server, and executed on a Linux victim machine. The activity was then monitored through QRadar to identify abnormal logs, system behavior, and network traffic.

---

## 🛠️ Tools & Technologies Used

- **MSFvenom** – for Trojan payload generation
- **Metasploit** – to establish and manage reverse shell sessions
- **Apache2 Server** – to host the malware
- **Linux OS** – as the victim environment
- **IBM QRadar SIEM** – for log monitoring and threat detection
- **Syslog & Network Logs** – for forensic analysis

---

## 🔍 Project Methodology

1. **Trojan Creation**: Payload generated using `msfvenom`
2. **Payload Hosting**: Served via local Apache web server
3. **Session Handling**: Reverse shell session created using Metasploit
4. **Execution**: Victim executed the malware on a Linux machine
5. **Monitoring**: QRadar analyzed logs, flows, and EPS spikes
6. **Detection**: QRadar flagged high-magnitude anomalies, showing internal system behavior and possible compromise

---

## 📊 QRadar Detection Highlights

- **Spike in Event Per Second (EPS)** after Trojan execution
- **Abnormal system notifications** from victim to loopback address
- **SAR threshold alerts** triggered and restored
- **Red magnitude bars** flagged suspicious log bursts
- **Timeline** showed the entire infection lifecycle, from execution to cleanup

---

## ✅ Key Learning Outcomes

- Real-time log monitoring with QRadar
- Malware behavior analysis through logs and flows
- Detection of reverse TCP connections via SIEM tools
- Importance of SAR alerts and correlation rules

---

## 📎 Full Project Report

[📄 Click here to view the complete PDF report](https://your-link-here.com)

> *(Replace with your actual link to Google Drive or GitHub-hosted PDF)*

---

## 🧠 Conclusion

This project effectively showcases how a SIEM like IBM QRadar can detect abnormal events caused by malware infections. Real-time log correlation, visual EPS spikes, and detailed system notifications provide a powerful method for identifying and responding to cyber threats.

---

## 📎 Full Project Report
[📄 Click here to view the full PDF report](https://drive.google.com/drive/folders/1gWxWYzt1oEVHc6JYdiB6PUUv57MkA6Sz?usp=drive_link)

