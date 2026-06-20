# ICMP Detection Simulation

## Date

20 June 2026

## Attack Type

ICMP Ping

## Attacker Machine

IdeaPad Kali Linux

## Defender Machine

ThinkPad VM running Snort 3

## Detection Rule

alert icmp any any -> any any (msg:"ICMP Ping Detected"; sid:1000001; rev:1;)

## Activity

The attacker machine generated ICMP traffic using the ping command against the defender machine.

## Result

Snort successfully detected and generated alerts for the ICMP traffic.

## Evidence

* 04-first-icmp-alert.png
* 05-ping-triggering-alert.png

## Learning

Custom Snort rules must be included in the active configuration before alerts can be generated. Successful alert generation confirmed that the IDS is functioning correctly.
