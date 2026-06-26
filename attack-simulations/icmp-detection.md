# ICMP Detection Simulation

## Date

20 June 2026

## Attack Type

ICMP Ping

## Lab Environment

### Attacker Machine

* IdeaPad running Kali Linux

### Defender Machine

* Ubuntu Virtual Machine running Snort 3 IDS
* Splunk Enterprise for SIEM and log analysis

## Detection Rule

```snort
alert icmp any any -> any any (msg:"ICMP Ping Detected"; sid:1000001; rev:1;)
```

## Attack Simulation

The Kali Linux attacker generated ICMP traffic using the `ping` command against the Ubuntu virtual machine running Snort 3.

## Detection

* Snort successfully detected the ICMP packets.
* Alerts were written to the Snort alert log.
* Splunk ingested the Snort alert log.
* The alerts were displayed in the Splunk dashboard.

## Splunk Dashboard

The dashboard includes:

* Total Snort Alerts
* ICMP Alerts
* Alert Timeline

## Evidence

* 04-first-icmp-alert.png
* 05-ping-triggering-alert.png
* 06-splunk-search-results.png
* 07-splunk-dashboard.png

## Learning

* Created and enabled a custom Snort ICMP detection rule.
* Verified successful attack detection using Snort.
* Forwarded Snort alerts into Splunk SIEM.
* Built a dashboard to visualize security events and attack timelines.
* Demonstrated a complete IDS-to-SIEM monitoring workflow.
