# Incident Report 02 - Port Scan Detection

## Date

21 June 2026

## Event Summary

A TCP port scan was launched from the attacker machine using Nmap. Snort 3 successfully detected the scan activity and generated alerts.

## Source

IdeaPad Kali Linux

## Destination

ThinkPad VM

## Attack Type

TCP SYN Port Scan

## Detection Rule

SID: 1000002

## Alert Message

Port Scan Detected

## Command Used

nmap 10.88.211.15

## Snort Statistics

* Packets Received: 14,667
* Packets Analyzed: 14,667
* Runtime: 00:02:17

## Result

Multiple alerts were generated during the scan.

## Lessons Learned

Port scanning is commonly used during reconnaissance. IDS solutions such as Snort can detect suspicious scanning behavior through custom detection rules.
