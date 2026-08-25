# 01 — Computer Networking Fundamentals

This is the foundation layer of networking. Before learning subnetting, VLANs, routing, Wireshark, firewalls, or cybersecurity networking, you should be comfortable with these concepts.

**What it is → why it exists → how it works → example → important details → common misconception.**

---

## 1. What Is a Computer Network?

**Simple definition**  
A computer network is a collection of devices connected together so they can communicate and exchange data or share resources.

**What can a network do?**  
Exchange files, access websites, send messages, share printers, share Internet access, access databases, run applications, make voice/video calls, access cloud services, monitor devices, and provide centralized services.

**What makes communication possible?**  
Devices → Network Interfaces → Communication Media → Protocols → Addresses → Networking Devices → Services.

---

## 2. Network Scope

| Type | Full Name | Scope | Example |
|------|-----------|-------|---------|
| **PAN** | Personal Area Network | Very small, around a person | Bluetooth headphones, smartwatch |
| **LAN** | Local Area Network | Limited area (home, office, building) | Home Wi-Fi, office switch |
| **WLAN** | Wireless Local Area Network | Wireless LAN | Home Wi-Fi |
| **MAN** | Metropolitan Area Network | City / metropolitan area | University campuses across a city |
| **WAN** | Wide Area Network | Large geographic area | Company connecting Manila–Cebu–Davao |

**Internet** = global network of networks.  
**Intranet** = private organizational network/resources (can still have Internet access behind a firewall).

---

## 3. Client, Server, Peer-to-Peer

- **Client** — requests a service (e.g., browser).
- **Server** — provides a service (web, DNS, file, DHCP, mail, etc.). Server is a *role*, not necessarily a special physical machine.
- **Peer-to-Peer (P2P)** — devices can act as both client and server and communicate directly without a central server.

One computer can be a client for one service and a server for another at the same time.

---

## 4. Network Topologies

- **Star** — devices connect to a central switch (most common in modern Ethernet LANs).
- **Bus** — shared medium (mostly historical).
- **Ring** — each device connects to neighbors.
- **Mesh** — multiple paths (full mesh requires $n(n-1)/2$ connections).
- **Hybrid** — combination of topologies (common in real networks).

Physical topology = cable/device layout.  
Logical topology = how data actually flows.

---

## 5. Performance Concepts

| Term | Meaning |
|------|---------|
| **Bandwidth** | Potential capacity of a link (Mbps / Gbps) |
| **Throughput** | Actual successful data transfer rate |
| **Latency** | Delay from source to destination (ms) |
| **Jitter** | Variation in packet delay |
| **Packet Loss** | Packets that fail to reach the destination |

Bandwidth ≠ Throughput. High bandwidth + high latency can still feel slow for interactive applications.

---

## 6. Duplex

- **Half-Duplex** — both directions possible, but not at the same time (walkie-talkie).
- **Full-Duplex** — both directions simultaneously (telephone). Modern switched Ethernet is full-duplex.

---

## 7. Delivery Models

| Model | Concept |
|-------|---------|
| **Unicast** | 1 → 1 |
| **Multicast** | 1 → selected group |
| **Broadcast** | 1 → everyone in the broadcast domain |
| **Anycast** | 1 → one of multiple possible instances (routing decides) |

---

## Mental Model

1. **WHAT** is communicating? → Hosts / Clients / Servers  
2. **WHERE** are they? → LAN / WAN / IP addressing  
3. **HOW** are they connected? → Ethernet / Wi-Fi / Fiber  
4. **HOW** does data move? → Packets / Frames / Protocols  
5. **WHERE** should it go? → Switching / Routing  
6. **HOW** fast/reliably? → Bandwidth / Throughput / Latency / Jitter / Packet Loss  
7. **WHO** should receive it? → Unicast / Multicast / Broadcast / Anycast  
8. **CAN** both sides communicate simultaneously? → Half / Full Duplex

---

## Checkpoint

1. Difference between LAN and WAN?  
2. Difference between Internet and Intranet?  
3. Can one computer be both client and server? Why?  
4. Main difference between client-server and P2P?  
5. Why is star topology common in modern LANs?  
6. Bandwidth vs Throughput?  
7. High bandwidth + high latency means?  
8. What is jitter?  
9. What happens when packets are lost?  
10. Half-duplex vs Full-duplex?  
11. Unicast / Multicast / Broadcast / Anycast differences?  
12. Phone on home Wi-Fi = LAN, WAN, or both?  
13. Why does a router matter for destinations outside the local network?  
14. Why isn’t “server” necessarily a specific type of physical computer?
