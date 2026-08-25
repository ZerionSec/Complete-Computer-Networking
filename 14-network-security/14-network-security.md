# 14 — Network Security

Security must be layered (**Defense in Depth**).

## Firewalls

- **Stateless** — filters on static rules only (IP/port).
- **Stateful** — tracks connection state; only allows return traffic that matches an existing flow.
- **Next-Generation (NGFW)** — Deep Packet Inspection, application awareness, threat intelligence.

## IDS / IPS

- **IDS** — detects and alerts (passive).
- **IPS** — detects and blocks (inline).

Detection methods: Signature-based, Anomaly-based, Policy-based.

## VPNs

- **Site-to-Site** — connects networks (often IPsec).
- **Remote Access** — connects individual users (IPsec, SSL/TLS, OpenVPN, WireGuard).

## Common Attacks & Mitigations

| Attack | Mitigation |
|--------|------------|
| ARP Spoofing / MITM | Dynamic ARP Inspection, DHCP Snooping |
| DDoS | Rate limiting, scrubbing centers, blackholing |
| VLAN Hopping | Hard-set ports, change native VLAN, disable DTP |
| Rogue DHCP | DHCP Snooping |

## Best Practices

Network Access Control (NAC), port security, least privilege, regular hardening, and continuous monitoring.
