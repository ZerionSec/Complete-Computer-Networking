# 04 — IPv4 Addressing & Subnetting

IPv4 is a 32-bit Layer 3 address written in dotted-decimal (e.g. `192.168.1.1`).

## Key Concepts

- **Network portion** vs **Host portion** (determined by the subnet mask / prefix length)
- **Network address** = first address (all host bits 0) — not assignable to hosts
- **Broadcast address** = last address (all host bits 1)
- **Usable hosts** = $2^n - 2$ where $n$ = number of host bits

## Special Addresses

| Type | Range / Value |
|------|---------------|
| Loopback | 127.0.0.0/8 (usually 127.0.0.1) |
| APIPA / Link-Local | 169.254.0.0/16 |
| Private (RFC 1918) | 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16 |
| Limited Broadcast | 255.255.255.255 |

## CIDR & Subnetting

- `/24` = 255.255.255.0 → 256 addresses, 254 usable
- Borrow host bits to create more subnets
- **VLSM** = different mask lengths for different subnets (efficient IP use)
- **Route summarization / Supernetting** = combine contiguous networks into one entry

### Quick Example

Network `192.168.1.0/24` → need 4 subnets  
→ borrow 2 bits → `/26` (mask 255.255.255.192)  
→ Block size 64  
→ Subnets: `.0/26`, `.64/26`, `.128/26`, `.192/26`  
→ 62 usable hosts each
