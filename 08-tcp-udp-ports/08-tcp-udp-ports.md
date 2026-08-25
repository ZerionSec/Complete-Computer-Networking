# 08 — TCP, UDP & Ports

## TCP (Transmission Control Protocol)

- Connection-oriented (3-way handshake)
- Reliable (sequence numbers, ACKs, retransmission)
- Flow control (window size) + congestion control
- Used by: HTTP/HTTPS, SSH, FTP, SMTP, etc.

## UDP (User Datagram Protocol)

- Connectionless, low overhead (8-byte header)
- Unreliable (no retransmissions)
- Used by: DNS, DHCP, VoIP, streaming, gaming, SNMP

## Ports

| Range | Name | Notes |
|-------|------|-------|
| 0–1023 | Well-Known | Require privileged rights (HTTP 80, HTTPS 443, SSH 22, DNS 53, etc.) |
| 1024–49151 | Registered | Applications (MySQL 3306, RDP 3389…) |
| 49152–65535 | Dynamic / Ephemeral | Temporary client-side ports |

A **socket** = IP address + Port.
