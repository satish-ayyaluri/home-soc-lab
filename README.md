# SOC Lab using Snort IDS and Splunk SIEM

## Project Overview

This project demonstrates a Security Operations Center (SOC) lab built using **Snort 3 IDS** and **Splunk Enterprise SIEM**. The lab simulates network attacks from a Kali Linux machine, detects them using Snort, forwards the alerts to Splunk, and visualizes security events through an interactive dashboard.

## Objectives

* Configure Snort 3 as a Network Intrusion Detection System (NIDS)
* Simulate network attacks from Kali Linux
* Detect ICMP traffic using custom Snort rules
* Ingest Snort alerts into Splunk Enterprise
* Build a SOC dashboard for security monitoring

## Lab Environment

| Component         | Purpose            |
| ----------------- | ------------------ |
| Kali Linux        | Attacker Machine   |
| Ubuntu 22.04 LTS  | Snort 3 IDS Sensor |
| Splunk Enterprise | SIEM Platform      |
| VirtualBox        | Virtualization     |

## Architecture

```text
Kali Linux
    │
    │ ICMP Ping Attack
    ▼
Ubuntu VM (Snort 3 IDS)
    │
    │ Alert Logs
    ▼
Splunk Enterprise
    │
    ▼
SOC Dashboard
```

## Attack Simulation

* ICMP Ping Attack
* Snort generated real-time alerts
* Splunk indexed Snort alert logs
* Dashboard displayed security events and alert timeline

## Dashboard Panels

* Total Network Alerts
* Live Log Feed
* ICMP Alerts
* Alert Timeline

## Project Outcome

Successfully built an end-to-end SOC monitoring lab that detects ICMP attacks, forwards alerts into Splunk Enterprise, and visualizes security events using a custom dashboard.

## Skills Demonstrated

* Network Security
* Snort 3 IDS
* Splunk Enterprise SIEM
* Log Analysis
* Linux Administration
* VirtualBox Networking
* Security Monitoring
* Cybersecurity Lab Setup
