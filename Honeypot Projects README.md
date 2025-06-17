# Honeypot Monitoring Using Cowrie and the ELK Stack

## Overview

This project focuses on detecting unauthorized access attempts by deploying a Cowrie honeypot integrated with the ELK Stack for real-time log analysis and visualization. The honeypot emulates an SSH/Telnet environment to attract attackers, while the ELK Stack (Elasticsearch, Logstash, Kibana) helps monitor and visualize attacker behavior through dashboards.

## Objective

- Deploy a medium-interaction honeypot using Cowrie
- Capture attacker interaction logs (credentials, commands, etc.)
- Forward logs using Filebeat to ELK Stack
- Use Kibana to create dashboards and analyze attack patterns
- Demonstrate how honeypots can support SOC-level threat intelligence

## Technologies Used

| Tool        | Purpose                                    |
|-------------|--------------------------------------------|
| Cowrie      | SSH/Telnet honeypot for capturing attacks  |
| Filebeat    | Log shipper to Elasticsearch               |
| Elasticsearch | Log storage and indexing               |
| Kibana      | Visual dashboards and log analysis         |
| Kali Linux  | Host machine for deployment                |

## Architecture Diagram (Text-Based)
Attacker
|
v
Cowrie Honeypot (SSH/Telnet Emulation)
|
v
Filebeat (Log Forwarder)
|
v
Elasticsearch -----> Kibana (Dashboards)

## Setup Summary

1. **Cowrie Installation**  
   - Installed using Git & Python venv  
   - Configured for JSON logging

2. **ELK Stack Installation**  
   - Installed Elasticsearch & Kibana on Kali  
   - Verified service status

3. **Filebeat Configuration**  
   - Configured to read Cowrie JSON logs  
   - Output to local Elasticsearch instance

4. **Testing and Visualization**  
   - Performed simulated SSH attacks  
   - Viewed captured data in Kibana Discover & Dashboards

## Key Visualizations in Kibana

- Source IP and geolocation of attacks
- Attempted login usernames/passwords
- Executed commands
- Frequency and timestamp distribution of attacks

## Outcome

This project successfully demonstrates the use of honeypots as a proactive security measure. By integrating Cowrie with the ELK Stack, real-time monitoring of attacker behavior becomes possible. The insights gained from these logs can assist in improving detection rules, refining network defenses, and generating threat intelligence for SOC teams.

## Full Report

[Download the full project report (PDF)](https://drive.google.com/file/d/174oMe6XikIO_Z9o0tVpaoLGE7MxFNjvt/view?usp=sharing)




