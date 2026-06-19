# Snort Verification

## Date

19 June 2026

## Objective

Verify that Snort can successfully capture and analyze network traffic in the SOC lab environment.

## Lab Environment

### Defender Machine

ThinkPad VM running Kali Linux with Snort 3

### Attacker Machine

IdeaPad running Kali Linux

### Network Configuration

* VirtualBox Bridged Adapter
* Monitored Interface: wlan0
* Defender IP: 10.88.211.15/24

## Activity Performed

1. Verified network connectivity between attacker and defender machines.
2. Configured VirtualBox networking using Bridged Adapter mode.
3. Started Snort packet capture on the defender machine.
4. Generated ICMP traffic from the attacker machine using the ping command.
5. Monitored packet statistics and interface activity.
6. Verified that Snort successfully processed live network traffic.

## Commands Used

### Defender Machine

```bash
sudo snort -v -i wlan0
```

### Attacker Machine

```bash
ping 10.88.211.15
```

## Results

* Network connectivity was successfully established between both machines.
* Snort successfully captured and analyzed network traffic on the monitored interface.
* Capture Duration: 90.99 seconds
* Packets Received: 225
* Average Packet Rate: 2 packets/second
* RX Bytes Received: 20,426
* Packet statistics confirmed that traffic generated from the attacker machine was successfully observed and processed by Snort.

## Observed Traffic Statistics

| Protocol | Packets |
| -------- | ------- |
| ARP      | 22      |
| ICMPv4   | 84      |
| ICMPv6   | 28      |
| IGMP     | 13      |
| IPv4     | 131     |
| IPv6     | 72      |
| UDP      | 78      |

## Troubleshooting

During the initial setup, Snort was not displaying packet information because of network configuration issues within VirtualBox. After switching to Bridged Adapter mode and verifying the correct interface (`wlan0`), packet capture was successfully validated.

## Evidence

Screenshots are available in the screenshots directory:

* 01-network-connectivity.png
* 02-snort-installed.png
* 03-snort-packet-capture.png

## Key Learning

This exercise demonstrated how Snort can be used as a Network Intrusion Detection System (NIDS) to monitor network traffic and provide visibility into network activity. It also highlighted the importance of proper network configuration, interface selection, and troubleshooting when deploying security monitoring tools.

## Conclusion

The SOC lab environment successfully captured and analyzed live network traffic between the attacker and defender systems. The Snort installation and network monitoring configuration have been verified and are ready for custom detection rules and alert generation in the next phase of the project.
