# 06 — VLANs (Virtual Local Area Networks)

A VLAN logically segments a physical switch into multiple isolated broadcast domains.

## Why VLANs?

- Security / isolation
- Smaller broadcast domains (better performance)
- Flexibility (logical grouping independent of physical location)
- Cost savings

## Key Concepts

- **Access Port** — belongs to one VLAN; frames leave untagged (end devices).
- **Trunk Port** — carries multiple VLANs; frames are tagged with **802.1Q** (4-byte tag containing VLAN ID).
- **Native VLAN** — untagged traffic on a trunk (default is VLAN 1). Best practice: change to an unused VLAN.
- Devices in different VLANs cannot communicate at Layer 2; they need a router or Layer-3 switch (inter-VLAN routing).

## Security Notes

- Disable Dynamic Trunking Protocol (DTP) and hard-set ports.
- Change native VLAN.
- Protect against VLAN hopping (double-tagging).
