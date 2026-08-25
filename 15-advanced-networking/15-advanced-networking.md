# 15 — Advanced Networking

## Software-Defined Networking (SDN)

Separates the **Control Plane** (decision-making) from the **Data Plane** (forwarding). A centralized SDN controller programs the switches via APIs (OpenFlow, etc.), making the network programmable and more flexible.

## Network Automation & IaC

- Tools: Ansible, Python (Netmiko/NAPALM), Puppet, Chef
- Protocols/Models: NETCONF / RESTCONF + YANG
- Goal: Zero-touch provisioning, reduced human error, Infrastructure as Code

## Network Virtualization / Overlays

- **VXLAN** — encapsulates L2 frames in UDP; 24-bit VNI (16 million segments vs VLAN’s 4096). Backbone of modern data centers.
- Other tunnels: GRE, Geneve

## BGP & MPLS

- **BGP** — the routing protocol of the Internet; policy-driven (AS-Path, Local Preference, MED).
- **MPLS** — label-based forwarding (Layer 2.5). Enables Traffic Engineering and L2/L3 VPNs.

## SD-WAN & Cloud Networking

- **SD-WAN** — abstracts multiple WAN links (MPLS, broadband, 4G/5G) into one logical fabric with application-aware routing.
- **Cloud** — VPCs / VNets, Security Groups, NACLs, Transit Gateways, Direct Connect / ExpressRoute (AWS, Azure, GCP).

## Observability

- Flow data: NetFlow / sFlow / IPFIX
- Streaming Telemetry (gRPC / Protobuf) for real-time visibility
