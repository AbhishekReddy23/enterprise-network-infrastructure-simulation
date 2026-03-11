<div align="center">

# Enterprise Network Infrastructure Simulation

![Status](https://img.shields.io/badge/status-completed-brightgreen)
![Type](https://img.shields.io/badge/project-network--engineering-blue)
![Platform](https://img.shields.io/badge/platform-kathara-lightgrey)

Enterprise-scale network simulation with routing, VPN connectivity, and security controls.

</div>

---

## Overview

This project implements a simulated enterprise network infrastructure using the **Kathara network emulator**.  
The objective was to design and deploy a complex multi-router environment capable of supporting routing, network services, and secure communication.

The project was developed as part of the **Network Infrastructures course** during my **Master's in Cybersecurity at Sapienza University of Rome**.

**Final Score:** 16/16

---

## Network Architecture

The simulated infrastructure consists of:

- 10 routers
- 3 servers
- 3 client machines

The environment is deployed using container-based network virtualization, enabling realistic testing of routing behavior and connectivity.

<img width="712" height="400" alt="image" src="https://github.com/user-attachments/assets/359b4b84-7199-4559-a86c-7b270dace2a1" />


---

## Implemented Features

- Multi-router network topology
- Dynamic routing configuration
- DHCP service deployment
- NAT gateway configuration
- Secure VPN connectivity
- Firewall rule implementation
- SSH secure access
- Network traffic capture and analysis

---

## Technologies Used

- Kathara (network emulation)
- Linux networking
- Routing protocols
- OpenVPN
- DHCP
- NAT
- SSH
- iptables
- tcpdump
- netcat

---

## Repository Structure

```text
enterprise-network-infrastructure-simulation
│
├── README.md
│
├── lab
│   ├── lab.conf
│   └── command.txt
│
├── configs
│   ├── routers
│   ├── clients
│   └── servers
│
├── topology.pdf
│   
└── captures

configs → configuration files for routers, clients, and servers

lab → Kathara lab configuration and commands

topology → network architecture diagram

Captures→ pcap data of clients for proof of working of network 
```
## Running the Lab

Start the network lab:

kathara lstart

Stop and clean the environment:

kathara lclean
## What I Learned

This project gave me hands-on experience designing and operating a production-style network in a virtualized environment. Key learning outcomes:

Designed and validated a multi-router topology with reliable end-to-end connectivity and subnet segmentation.

Implemented and troubleshot routing (OSPF/static), DHCP, and NAT to ensure correct inter-site reachability.

Deployed PKI-backed OpenVPN tunnels and verified encrypted traffic flows using packet captures.

Hardened host and network configurations using SSH key authentication and iptables firewall rules.

Used tcpdump and targeted traffic generation to validate detection scenarios and confirm that security controls enforced intended policies.

## Improved troubleshooting workflow: 
rapid isolation of routing or ACL faults, reproducible test cases, and documentation of remediation steps.

## Academic outcome: Full marks (16/16) for the Network Infrastructures course.

## Skills Demonstrated:

Network Architecture & Design

Routing Protocols (OSPF / static routing)

VPN Deployment (OpenVPN, PKI)

Linux Networking Administration

DHCP, NAT, and IP Address Management

Firewall Configuration (iptables) & Access Control

Packet Capture & Analysis (tcpdump, .pcap)

Network Troubleshooting & Test Automation (netcat, scripted tests)

Infrastructure Documentation & Reproducible Labs

## Author

Abhishek Reddy Gade
Master's in Cybersecurity — Sapienza University of Rome
