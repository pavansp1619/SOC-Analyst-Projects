# 🛡️ Intrusion Detection and Prevention using Suricata on pfSense Firewall

## 📌 Project Overview

This project showcases how to implement a real-time **Intrusion Detection and Prevention System (IDS/IPS)** using 🧠 **Suricata** and 🔥 **pfSense firewall**. It simulates common cyberattacks (like port scanning and web scanning) using Kali Linux and demonstrates how Suricata detects and blocks threats in both IDS and IPS modes.

By integrating open-source tools in a virtual lab environment, this project helps build practical knowledge in threat detection, network monitoring, and SOC operations.

---

## 🎯 Objectives

- 🚀 Deploy Suricata on pfSense firewall
- 🧪 Simulate cyberattacks from Kali Linux
- 📊 Monitor alerts in IDS mode
- ⛔ Block malicious traffic in IPS mode
- ⚙️ Configure rule sets and analyze alerts
- 🔁 Understand real-time traffic behavior

---

## 🛠️ Tools & Technologies Used

| 🔧 Tool         | 📝 Purpose                                      |
|----------------|------------------------------------------------|
| 🖥️ pfSense      | Open-source firewall and routing platform     |
| 🔐 Suricata     | Network-based IDS/IPS engine                  |
| 🐍 Kali Linux   | Attack simulation environment                 |
| 🔍 Nmap         | Stealth scanning tool                         |
| 🌐 Nikto        | Web vulnerability scanner                     |

---

## 🧱 Setup Summary

### 🧰 Environment Setup

| 💻 Component     | ⚙️ Configuration                          |
|------------------|--------------------------------------------|
| pfSense          | With Suricata installed                   |
| Suricata         | Legacy (IDS) and Inline (IPS) Modes       |
| Kali Linux VM    | Host-only network (IP: 192.168.1.101)     |
| Target IP        | pfSense LAN (192.168.1.1)                 |

---

### 🪜 Key Steps

1. 📥 Download & install pfSense ISO in VirtualBox
2. 🔌 Configure two network adapters (WAN & LAN)
3. 🌐 Access pfSense UI (http://192.168.1.1) from Kali
4. 🧩 Install Suricata package via pfSense Package Manager
5. 🧾 Enable **Emerging Threats** rules and `eve.json` logging
6. 🧪 Simulate attacks:
   - `nmap -sS 192.168.1.1` (stealth scan)
   - `nikto -h http://192.168.1.1` (HTTP scan)
7. 🧠 Review alerts in Suricata dashboard & logs
8. 🔒 Enable IPS mode for active blocking

---

## 📈 Results

- ✅ Suricata detected:
  - 🔍 Port scans via Nmap
  - 🌐 Web scans via Nikto
- 📋 IDS Mode: Logged alerts without blocking
- ⛔ IPS Mode: Detected and blocked threats in real time
- 🗂 Logs analyzed via `/var/log/suricata/` and pfSense web UI

---

## 🧠 Key Takeaways

- 🔐 IDS/IPS tools provide critical visibility into network threats
- ⚙️ Proper rule configuration ensures accurate detection
- 📡 pfSense + Suricata is a powerful open-source combo for SOCs
- 💡 Real-time monitoring strengthens incident response capability

---

## 📎 Full Report

[📄 Click here to view the full project report (PDF)](https://drive.google.com/file/d/1L1clHGTgzt0xzW16Cj9ty3N5bpWNu4il/view?usp=sharing)


