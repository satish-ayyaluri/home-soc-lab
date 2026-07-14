# 🛡️ Home Security Operations Center (SOC) Lab using Snort 3 IDS and Splunk Enterprise SIEM

![Platform](https://img.shields.io/badge/Platform-Ubuntu-orange)
![IDS](https://img.shields.io/badge/IDS-Snort3-red)
![SIEM](https://img.shields.io/badge/SIEM-Splunk-green)
![Virtualization](https://img.shields.io/badge/VirtualBox-Lab-blue)

---

# 📖 Project Overview

This project demonstrates a complete **Security Operations Center (SOC)** lab built using **Snort 3 IDS** and **Splunk Enterprise SIEM**. The lab simulates network attacks from a Kali Linux machine, detects them using Snort, forwards alerts to Splunk, and visualizes security events through an interactive SOC dashboard.

---

# 🎯 Objectives

- Configure Snort 3 as a Network Intrusion Detection System (NIDS)
- Simulate network attacks from Kali Linux
- Detect ICMP traffic using custom Snort rules
- Forward Snort alerts to Splunk Enterprise
- Build a SOC dashboard for security monitoring
- Analyze security events and alerts

---

# 🛠️ Technologies Used

- Ubuntu 22.04 LTS
- Kali Linux
- Snort 3 IDS
- Splunk Enterprise SIEM
- VirtualBox
- Linux CLI
- TCP/IP
- ICMP

---

# 🖥️ Lab Environment

| Component | Purpose |
|----------|---------|
| Kali Linux | Attacker Machine |
| Ubuntu 22.04 LTS | Snort 3 IDS Sensor |
| Splunk Enterprise | SIEM Platform |
| VirtualBox | Virtualization |

---

# 🏗️ Lab Architecture

```
Kali Linux (Attacker)
        │
        │ ICMP Ping Attack
        ▼
Ubuntu VM (Snort 3 IDS)
        │
        │ Alert Logs
        ▼
Splunk Enterprise SIEM
        │
        ▼
SOC Dashboard
```

---

# 🔍 Custom Snort Detection Rule

```snort
alert icmp any any -> $HOME_NET any (msg:"ICMP Ping Detected"; sid:1000001; rev:1;)
```

---

# ⚔️ Attack Simulation

- ICMP Ping Attack from Kali Linux
- Snort generated real-time intrusion alerts
- Splunk indexed Snort alert logs
- Dashboard displayed live security events
- Alert timeline visualized attack activity

---

# 📊 SOC Dashboard

![SOC Dashboard](/screenshots/soc-dashboard.jpeg)



```markdown
![SOC Dashboard](images/soc-dashboard.png)
```

---

# 📈 Dashboard Panels

- Total Network Alerts
- Live Log Feed
- ICMP Detection Alerts
- Alert Timeline
- Security Event Monitoring

---

# ✅ Project Outcome

Successfully designed and implemented an end-to-end Home Security Operations Center (SOC) lab capable of detecting ICMP attacks, forwarding Snort alerts into Splunk Enterprise, and visualizing security events using a custom SOC dashboard.

---

# 💡 Skills Demonstrated

- Security Operations Center (SOC)
- Snort 3 IDS
- Splunk Enterprise SIEM
- Intrusion Detection
- Log Analysis
- Network Security
- Linux Administration
- VirtualBox Networking
- TCP/IP
- Cybersecurity Lab Setup

---

# 🚀 Future Enhancements

- Detect TCP and UDP attacks
- Add SSH Brute Force Detection
- Integrate Zeek
- Configure Syslog Forwarding
- Create Advanced Splunk Dashboards
- Develop Additional Custom Snort Rules

---

## 👨‍💻 Author

**Ayyaluri Satish Kumar Reddy**

Aspiring SOC Analyst | Cybersecurity Enthusiast | Python Learner | Google Cybersecurity Professional Certificate 
