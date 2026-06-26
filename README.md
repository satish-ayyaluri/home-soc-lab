# SOC Lab using Snort IDS and Splunk SIEM

## Project Overview

This project demonstrates a Security Operations Center (SOC) lab built using **Snort IDS** and **Splunk SIEM**. The lab detects network attacks, stores alerts, and visualizes security events through a Splunk dashboard.

## Objectives

* Configure Snort as a Network Intrusion Detection System (NIDS)
* Simulate attacks from Kali Linux
* Collect Snort alerts in Splunk
* Build a dashboard to monitor security events

## Technologies Used

* Ubuntu Linux
* Kali Linux
* Snort IDS
* Splunk Enterprise
* VirtualBox

## Architecture

Kali Linux (Attacker)
↓ ICMP Ping Attack
Ubuntu + Snort IDS
↓ Alert Logs
Splunk Enterprise
↓
Dashboard & Security Monitoring

## Attack Simulation

* ICMP Ping Attack
* Snort generated alerts
* Splunk indexed alert logs
* Dashboard displayed attack events and timeline

## Dashboard Panels

* Total Snort Alerts
* ICMP Alerts
* Alert Timeline

## Project Outcome

Successfully built a functional SOC lab capable of detecting ICMP attacks, forwarding alerts to Splunk, and visualizing security events through dashboards.

## Skills Demonstrated

* Network Security
* Intrusion Detection
* SIEM Monitoring
* Log Analysis
* Linux Administration
* Cybersecurity Lab Setup
