# 🛡️ Malware Detection and Log Analysis using QRadar SIEM

## 🔍 Project Overview
This project demonstrates how malware activity can be detected using IBM QRadar SIEM. A Trojan payload was created using MSFvenom, delivered to a Linux machine, and monitored for abnormal system behavior.

## 🧰 Tools Used
- MSFvenom
- Metasploit Framework
- Apache Server
- IBM QRadar SIEM
- Linux OS

## ⚙️ Steps Performed
1. Generated a Trojan payload using `msfvenom`.
2. Hosted the payload using Apache on Kali Linux.
3. Created a reverse TCP session using Metasploit.
4. Monitored system and network behavior via QRadar.

## 📸 Screenshots

### 🧪 Payload Creation using MSFvenom
![Payload Creation](./images/page_4_img_1.jpeg)

### 🌐 Payload Hosted on Apache Server
![Apache Hosting](./images/page_5_img_1.png)

### 💻 Reverse TCP Connection Setup
![Metasploit Listener](./images/page_5_img_2.png)

### 📈 QRadar Log Spike Detection
![QRadar EPS Spike](./images/page_6_img_1.jpeg)

### ⚠️ QRadar Alert Details
![QRadar Alerts](./images/page_6_img_2.jpeg)

## 📈 Results
- EPS and event count spiked after payload execution.
- QRadar flagged system notification floods.
- Internal communications were traced via logs.

## 👤 Author
**Pavan M G**

📄 [Full Project Report](./report/QRadar_Project_Report.pdf)

