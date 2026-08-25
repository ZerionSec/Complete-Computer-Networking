# 03 — Ethernet & MAC Addressing

Ethernet (IEEE 802.3) is the foundational technology for wired LANs.

## Ethernet Frame Structure

| Field | Size | Purpose |
|-------|------|---------|
| Preamble + SFD | 8 bytes | Synchronization |
| Destination MAC | 6 bytes | Who this is for |
| Source MAC | 6 bytes | Who sent this |
| EtherType / Length | 2 bytes | Upper-layer protocol (0x0800 = IPv4, 0x0806 = ARP) or length |
| Payload | 46–1500 bytes | Actual data (IP packet, etc.) |
| FCS | 4 bytes | CRC-32 error detection |

## MAC Address

- 48-bit (6-byte) address, written as `MM:MM:MM:SS:SS:SS`
- First 3 bytes = OUI (manufacturer)
- Last 3 bytes = device-specific
- Layer 2 only — used within the same local segment / broadcast domain; does **not** cross routers

**Unicast / Multicast / Broadcast**  
The least-significant bit of the first byte: 0 = Unicast, 1 = Multicast. Broadcast = `FF:FF:FF:FF:FF:FF`.

## Key Takeaway

MAC addresses are physical (burned into NIC) but only meaningful on the local link. Every router hop replaces the MAC addresses while the IP addresses stay the same.
