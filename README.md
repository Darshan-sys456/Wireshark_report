# Wireshark Network Traffic Analysis

## Project Overview

This project focuses on capturing and analyzing real-time network traffic using **Wireshark**, a widely used network protocol analyzer.

The analysis examines captured packets, protocol hierarchy, IPv4 endpoints, and IP conversations to understand communication between a local system and external network devices.

## 1. Capture Information

| Parameter | Details |
|---|---|
| Tool | Wireshark |
| Capture Date | 23 November 2026 |
| Capture Time | 10:44:38 AM IST |
| Total Packets | 59 |
| Network Interface IP | 192.168.28.128 |
| Analysis Type | Network Traffic Analysis |

## 2. Protocol Hierarchy

The captured traffic contains the following protocols:

| Protocol | Frames | Bytes |
|---|---:|---:|
| Ethernet | 59 | 18,312 |
| ARP | 4 | 240 |
| IPv4 | 55 | 18,072 |
| UDP | 4 | 697 |
| DNS | 4 | 697 |
| TCP | 51 | 17,375 |
| TLS | 16 | 8,041 |

### Protocol Distribution

- **Ethernet:** Used for local network frame transmission.
- **ARP:** Used for IPv4-to-MAC address resolution.
- **IPv4:** Responsible for logical addressing and routing.
- **UDP:** Used for connectionless communication.
- **DNS:** Handles domain name resolution.
- **TCP:** Provides reliable and ordered data transmission.
- **TLS:** Provides encrypted communication.

## 3. IP Endpoint Analysis

The following IPv4 endpoints were identified:

| IP Address | Packets | Bytes |
|---|---:|---:|
| 192.168.28.128 | 55 | 18 kB |
| 150.171.27.10 | 35 | 15 kB |
| 150.171.110.84 | 7 | 522 bytes |
| 20.85.17.170 | 5 | 282 bytes |
| 192.168.28.2 | 4 | 697 bytes |
| 150.171.110.87 | 4 | 870 bytes |

**Local System:** `192.168.28.128`

The endpoint statistics show communication between the local system and multiple network endpoints.

## 4. IP Conversation Analysis

A total of five IPv4 conversations were identified.

| Communication | Total Frames | Total Bytes | Duration |
|---|---:|---:|---:|
| 192.168.28.128 ↔ 150.171.27.10 | 35 | 15 kB | 1.2658 s |
| 150.171.110.84 ↔ 192.168.28.128 | 7 | 522 bytes | 0.0030 s |
| 192.168.28.128 ↔ 20.85.17.170 | 5 | 282 bytes | 1.2805 s |
| 192.168.28.2 ↔ 192.168.28.128 | 4 | 697 bytes | 0.0013 s |
| 192.168.28.128 ↔ 150.171.110.87 | 4 | 870 bytes | 0.1030 s |

## 5. Analysis Observations

1. A total of 59 packets were successfully captured.
2. Ethernet was the underlying link-layer protocol.
3. Four ARP packets were observed.
4. IPv4 accounted for 55 packets.
5. DNS communication was observed through UDP.
6. TCP was the most frequently observed transport protocol.
7. TLS packets indicate encrypted network communication.
8. The local system communicated with multiple IPv4 endpoints.
9. The largest observed conversation involved `192.168.28.128` and `150.171.27.10`.

## 6. Tools and Technologies

- Wireshark
- Network Protocol Analysis
- IPv4
- TCP/IP
- DNS
- ARP
- TLS

## 7. Conclusion

The Wireshark traffic analysis provided an overview of network communication generated during the capture session.

The captured data helped identify different protocols, inspect IPv4 endpoints, and understand communication between the local system and external endpoints.

This practical analysis demonstrates how Wireshark can be used for network monitoring, troubleshooting, protocol identification, and cybersecurity learning.

---

**Project Type:** Practical Network Traffic Analysis  
**Tool Used:** Wireshark  
**Purpose:** Educational and Cybersecurity Research
