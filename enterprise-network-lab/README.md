
# Enterprise Network Lab (Packet Tracer)

A small enterprise network demonstrating VLANs, inter‑VLAN routing (router‑on‑a‑stick), DHCP, and a security-focused variant (Port Security, DHCP Snooping, DAI, SSH, and Zone-Based Firewall basics).

## Topology
- R1 (Router)
- S1 (2960 Switch)
- PC0 (VLAN 10)
- PC1 (VLAN 20)

See `diagrams/topology.png` (export your Packet Tracer diagram there).

## How to Use
1. Open Packet Tracer and recreate the topology (or use your `.pkt` file if you save one).
2. Apply configs from `configs/` for the base lab.
3. Apply configs from `security-version/` to enable security features.

## Verification
- `ping` between VLANs
- `show vlan brief`, `show interfaces trunk`
- `show ip interface brief` on R1
- For security: `show port-security interface fa0/1`, `show ip dhcp snooping`, `show ip arp inspection`

## Author
Prepared by Njabulo Ntshangase.
