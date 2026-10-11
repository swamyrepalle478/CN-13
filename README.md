# CN-13
# Wireshark Network Protocol Analysis

## Aim

To study Wireshark, capture network packets, analyze protocols, apply filters, and understand network traffic statistics.

## Objectives

* Understand network protocol analysis using Wireshark.
* Capture and save network traffic.
* Identify source and destination addresses.
* Analyze TCP, UDP, ICMP, IPv4, IPv6, and ARP packets.
* Filter packets using IP addresses and protocols.
* Generate basic protocol statistics.

## Requirements

* Python 3
* Wireshark
* Scapy Python library
* A saved PCAP or PCAPNG capture file

## Installation

Install Scapy using:

```bash
python -m pip install scapy
```

Download Wireshark from https://www.wireshark.org/.

## Execution

Run the program:

```bash
python wireshark_analysis.py
```

Enter the path to your saved `.pcap` or `.pcapng` file.

## Features

1. Reads saved packet capture files.
2. Displays packet timestamps, source and destination addresses, protocol, and length.
3. Counts packets by protocol.
4. Summarizes source addresses.
5. Filters packets using IP addresses.
6. Displays packets belonging to TCP, UDP, or ICMP.

## Wireshark Filters

Examples of display filters:

* `tcp`
* `udp`
* `icmp`
* `arp`
* `ip.addr == 192.168.1.10`
* `tcp.port == 443`
* `dns`

Examples of capture filters:

* `host 192.168.1.10`
* `tcp port 443`
* `udp port 53`

## Result

The program analyzes a saved packet capture, displays packet information, applies IP and protocol filters, and produces basic protocol statistics.

Note: Capture traffic only on networks and devices you are authorized to analyze. This Python program analyzes saved captures; live packet capture and advanced statistics are available in Wireshark itself.
