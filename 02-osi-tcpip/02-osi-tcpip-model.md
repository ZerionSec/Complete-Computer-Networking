# 02 — OSI Model + TCP/IP Model

The real goal is to understand: **How does data move from one application on one computer to an application on another computer?**

---

## Why Layers?

Networking is divided into layers so each layer has a clear responsibility. This makes design, implementation, and troubleshooting manageable.

---

## OSI 7-Layer Model

| Layer | Name | Main Idea | Examples |
|-------|------|-----------|----------|
| 7 | Application | Network services for applications | HTTP, DNS, SMTP, SSH |
| 6 | Presentation | Data representation | Encoding, encryption concepts |
| 5 | Session | Communication sessions | Session management concepts |
| 4 | Transport | End-to-end transport | TCP, UDP |
| 3 | Network | Logical addressing & routing | IP, routers |
| 2 | Data Link | Local-link communication | Ethernet, MAC, switches |
| 1 | Physical | Signals / bits | Copper, fiber, radio |

**Mnemonic:** All People Seem To Need Data Processing

---

## TCP/IP Model (4-layer)

| TCP/IP | Rough OSI Mapping |
|--------|-------------------|
| Application | Layers 5–7 |
| Transport | Layer 4 |
| Internet | Layer 3 |
| Link | Layers 1–2 |

---

## Encapsulation & Decapsulation

As data goes **down** the stack, each layer adds its header → **Encapsulation**.  
As data goes **up** the stack on the receiver → **Decapsulation**.

**PDUs:**

- Layers 5–7 → Data  
- Layer 4 → Segment (TCP) / Datagram (UDP)  
- Layer 3 → Packet  
- Layer 2 → Frame  
- Layer 1 → Bits

---

## Critical Rule

**IP addresses (Layer 3) stay the SAME from source to destination.**  
**MAC addresses (Layer 2) CHANGE at every router hop.**

Analogy: IP = final home address. MAC = next post-office stop label.

---

## Packet Journey (Simplified)

1. **PC** creates HTTP request → TCP segment → IP packet → Ethernet frame (Src MAC = PC, Dst MAC = Gateway).
2. **Switch** forwards based on Destination MAC (does not change IP or MAC).
3. **Router** strips L2 frame, looks at Destination IP, finds next hop, builds a **new** frame with new Src/Dst MAC, forwards.
4. Process repeats at every router until the destination server.
5. Server decapsulates up the stack and hands data to the application.

---

## TCP Three-Way Handshake

1. **SYN** — Client: “I want to talk. Seq = X”
2. **SYN-ACK** — Server: “Got X. My Seq = Y”
3. **ACK** — Client: “Got Y. Connection ready.”

Needed so both sides agree and old delayed SYNs don’t confuse the server.

---

## Why Professionals Still Use OSI

It gives a common troubleshooting vocabulary:

- Layer 1 problem → cable, signal, interface  
- Layer 2 problem → MAC, VLAN, switching  
- Layer 3 problem → IP, subnet, routing, gateway  
- Layer 4 problem → TCP/UDP, ports, connections

Always start from the bottom when troubleshooting.

---

## Checkpoint

1. What is the OSI model?  
2. Why divide networking into layers?  
3–7. Responsibilities of Layers 1, 2, 3, 4, and 7?  
8. MAC vs IP address?  
9. What is encapsulation / decapsulation?  
10. Frame vs Packet vs Segment?  
11. Why does a router mainly operate at Layer 3?  
12. Why does a switch mainly operate at Layer 2?
