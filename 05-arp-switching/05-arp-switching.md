# 05 — ARP & Switching

## ARP (Address Resolution Protocol)

Resolves IP (Layer 3) → MAC (Layer 2) on the local segment.

1. Host checks ARP cache.
2. If missing → broadcasts ARP Request: “Who has IP X?”
3. Owner replies with unicast ARP Reply containing its MAC.
4. Cache is updated; frame can now be sent.

**Security note:** ARP has no authentication → vulnerable to ARP Spoofing / Poisoning (MITM).

## Switching (Layer 2)

A switch builds a **MAC Address Table (CAM table)** by learning source MACs of incoming frames.

**Actions:**
- **Flood** — unknown unicast or broadcast
- **Forward** — known destination on different port
- **Filter** — destination is on the same port as source

**STP (Spanning Tree Protocol)** prevents Layer-2 loops by blocking redundant paths and reactivating them on failure.

**Switching methods:** Store-and-Forward (checks FCS), Cut-Through (lowest latency), Fragment-Free.
