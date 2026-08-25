# 🌐 Complete Computer Networking

A comprehensive Computer Networking self-learning repository designed to build networking knowledge from foundational concepts to advanced and modern networking technologies.

This repository covers the complete networking learning path—from understanding what a network is and how packets travel, to subnetting, switching, routing, wireless networking, network security, cloud networking, automation, and advanced network architectures.

---

## 📚 What You'll Learn

### 1. 🧱 The Foundations — Topics 01–03

The foundation of computer networking, including:

- Network, Node, Host, Client, and Server
- LAN, WAN, MAN, PAN
- Internet vs. Intranet
- Network topologies: Star, Bus, Ring, Mesh
- Network performance: Bandwidth, Throughput, Latency, Jitter, Packet Loss
- Duplex communication
- Network delivery models: Unicast, Broadcast, Multicast, Anycast
- OSI 7-Layer Model
- TCP/IP Model
- Encapsulation and decapsulation
- How a packet travels from a client device to a web server

### 2. 🔌 Core Networking Infrastructure — Topics 04–15

The core technologies used to build and operate modern networks.

**Layer 2 — Data Link**  
Ethernet · Ethernet Frames · MAC Addresses · MAC Address Tables · Switching · CAM Tables · STP · VLANs · 802.1Q Trunking · Access and Trunk Ports · ARP

**Layer 3 — Network**  
IPv4 Addressing · Network and Host Portions · Private and Special-Purpose Addresses · Subnet Masks · Subnetting · CIDR · VLSM · Route Summarization · IPv6 Addressing · IPv6 Address Types · NDP · SLAAC · Static Routing · Dynamic Routing · OSPF · BGP

**Layer 4 — Transport**  
TCP · UDP · TCP 3-Way Handshake · Sequence and Acknowledgment Numbers · Flow Control · Congestion Control · TCP Flags · Network Ports · Well-Known, Registered, and Ephemeral Ports

**Network Services**  
DNS · DNS Resolution · DNS Records · DNS Caching and TTL · DHCP · DHCP DORA Process · DHCP Relay

**Connectivity**  
NAT · PAT / NAT Overload · Static NAT · Dynamic NAT · Wireless Networking · Wi-Fi Standards · 2.4 GHz / 5 GHz / 6 GHz · Wi-Fi 6 / 6E · Wireless Security

**Troubleshooting**  
Ping · Traceroute / Tracert · IP configuration tools · ARP inspection · DNS troubleshooting · TCP/UDP connectivity testing · Netstat / ss · Wireshark · Packet capture and analysis · TCP stream analysis

### 3. 🛡️ Advanced Networking & Security — Topics 16–18

The final stage focuses on protecting, automating, scaling, and modernizing networks.

**Network Security**  
Network Security Fundamentals · Firewalls (Stateless, Stateful, Next-Generation) · IDS/IPS · VPNs · Network Access Control · Defense in Depth · ARP Spoofing · Man-in-the-Middle Attacks · DDoS Attacks · VLAN Hopping · DHCP Snooping · Dynamic ARP Inspection · Network Hardening

**Advanced Networking**  
Software-Defined Networking (SDN) · Control Plane vs. Data Plane · Network Automation · Infrastructure as Code · Python for Network Automation · Ansible · REST APIs · NETCONF / RESTCONF · YANG · Network Virtualization · Overlay and Underlay Networks · VXLAN · EVPN · GRE / Geneve · BGP · MPLS · Traffic Engineering · SD-WAN · Cloud Networking (AWS / Azure / GCP) · VPC / VNet · Security Groups · Network ACLs · Transit Gateways · Network Observability · NetFlow / IPFIX · Streaming Telemetry

---

## 🎯 Learning Objectives

By completing this repository, you should be able to:

- Explain how computer networks operate.
- Understand the OSI and TCP/IP models.
- Understand how Ethernet frames and IP packets move through a network.
- Configure and calculate IPv4 subnets.
- Understand IPv6 addressing and routing.
- Explain how switches and routers make forwarding decisions.
- Understand VLANs and inter-VLAN communication.
- Understand TCP, UDP, ports, and common network services.
- Troubleshoot common network connectivity and DNS problems.
- Capture and analyze network traffic using Wireshark.
- Understand fundamental network security controls.
- Understand modern technologies such as SDN, VXLAN, BGP, MPLS, SD-WAN, and cloud networking.
- Build practical networking knowledge through hands-on labs.

---

## 🧪 Hands-On Learning

This repository is intended to go beyond memorization.

Recommended laboratory environments include:

- Cisco Packet Tracer
- GNS3
- EVE-NG
- Wireshark
- Linux virtual machines
- Virtual network laboratories
- Authorized test environments

The goal is to progress from **theory → configuration → troubleshooting → security → advanced networking**.

---

## 🗺️ Learning Path

```
FOUNDATIONS
   ↓
OSI & TCP/IP
   ↓
ETHERNET & MAC
   ↓
IPv4 & SUBNETTING
   ↓
ARP & SWITCHING
   ↓
VLANs
   ↓
ROUTING
   ↓
TCP / UDP / PORTS
   ↓
DNS & DHCP
   ↓
NAT
   ↓
IPv6
   ↓
WIRELESS
   ↓
TROUBLESHOOTING & WIRESHARK
   ↓
NETWORK SECURITY
   ↓
ADVANCED NETWORKING
   ↓
AUTOMATION & CLOUD
   ↓
HANDS-ON LABS
   ↓
NETWORK PROJECTS
```

---

## 📁 Repository Structure

```
/
├── 01-foundations/                 # Network basics, topologies, performance
├── 02-osi-tcpip/                   # OSI Model + TCP/IP Model + Encapsulation
├── 03-ethernet-mac/                # Ethernet frames, MAC addressing
├── 04-ipv4-subnetting/             # IPv4, CIDR, VLSM, Subnetting
├── 05-arp-switching/               # ARP, Switching, CAM, STP
├── 06-vlans/                       # VLANs, 802.1Q, Trunking
├── 07-routing/                     # Static & Dynamic Routing, OSPF, BGP
├── 08-tcp-udp-ports/               # TCP, UDP, Ports, Handshake
├── 09-dns-dhcp/                    # DNS, DHCP, DORA
├── 10-nat/                         # NAT, PAT, Static/Dynamic NAT
├── 11-ipv6/                        # IPv6 Addressing, NDP, SLAAC
├── 12-wireless/                    # Wi-Fi Standards, Security
├── 13-troubleshooting-wireshark/   # Tools + Packet Analysis
├── 14-network-security/            # Firewalls, VPNs, Attacks, Hardening
├── 15-advanced-networking/         # SDN, VXLAN, BGP, MPLS, SD-WAN, Cloud
├── labs/                           # Packet Tracer / GNS3 / Lab notes
└── README.md
```

---

## ⚖️ Legal & Ethical Use

This repository is intended for **education, self-learning, laboratory practice, and authorized network administration**.

Only perform network testing, packet capture, scanning, configuration changes, or security assessments on systems and networks that you **own** or have **explicit permission** to test.

**Do not** use the material to disrupt, access, intercept, or attack unauthorized systems.

---

## 🚀 Goal

The ultimate goal of this repository is to provide a structured path from beginner networking concepts to advanced professional-level networking knowledge, while combining theory with practical laboratory experience.

**Learn → Build → Analyze → Troubleshoot → Secure → Automate.**

---

## 📬 Connect

If you find this useful, feel free to ⭐ the repository and open issues for suggestions or corrections.

---

**Disclaimer:** This is an independent educational resource. It is not affiliated with, endorsed by, or connected to any certification body or vendor.
