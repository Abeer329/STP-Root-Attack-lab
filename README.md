# STP-Root-Attack-lab
STP Root Attack and BPDU Guard security lab using Cisco switches and kali Linux
# STP Root Attack Lab

## Overview
This project demonstrates a Spanning Tree Protocol (STP) Root Attack using Yersinia against Cisco switches in GNS3.

The attacker attempts to become the Root Bridge by sending rogue BPDU packets.

BPDU Guard is then configured to automatically detect and block the malicious interface.

---

## Technologies Used
- Cisco IOSv-L2
- GNS3
- Kali Linux
- Yersinia
- STP
- BPDU Guard

---

## Attack Demonstration
The attacker used Yersinia to launch a rogue BPDU attack and attempt Root Bridge takeover.

---

## Protection Mechanism

```cisco
interface gi0/2
 spanning-tree portfast
 spanning-tree bpduguard enable

