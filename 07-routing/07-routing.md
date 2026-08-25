# 07 — Routing

Routing = forwarding packets between different networks (Layer 3) using IP addresses.

## Routing Table & Longest Prefix Match

Router looks up Destination IP and chooses the most specific matching route.

## Types of Routing

| Type | Description |
|------|-------------|
| **Static** | Manually configured. Simple but does not scale. |
| **Default Route** | `0.0.0.0/0` — gateway of last resort. |
| **Dynamic** | Routers share information automatically. |

### Dynamic Protocols

- **Distance-Vector** (RIP, EIGRP) — shares routes with neighbors; hop-count or composite metric.
- **Link-State** (OSPF, IS-IS) — builds full topology map, runs SPF (Dijkstra).
- **Path-Vector** (BGP) — internet backbone protocol; policy-based (AS-Path, Local Preference, MED).

## Key Router Actions

1. Extract Destination IP
2. Longest-prefix match in routing table
3. Decrement TTL, recalculate checksum
4. Rewrite Layer-2 MAC addresses for the next hop
5. Forward out the exit interface
