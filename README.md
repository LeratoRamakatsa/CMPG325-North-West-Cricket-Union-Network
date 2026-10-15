# CMPG325-North-West-Cricket-Union-Network

CMPG325 -- North-West Cricket Union Network
Module: CMPG325 Computer Networks
Project: Individual Semester Project
Client: North-West Cricket Union
Location: South Africa
Student: Lerato Ramakatsa
Student number: 35840544
Assigned feature: Router-on-a-Stick Inter-VLAN Routing

Project Overview
The project uses Cisco Packet Tracer to develop and deploy a network for the Northwest Cricket Union. Five departmental PCs (CR1, CR5), a router, a central switch, and a shared printer are on the network.This design divides departments into VLANs and traffic is routed between them via a router-to-switch link. Topology, IP strategy, implementation, verification, and troubleshooting are covered in the documentation.

IP addressing plan
The assigned block is 192.168.51.0/24. The design uses /27 subnets
with subnet mask 255.255.255.224. Each /27 has 30 usable host
addresses.

VLAN           Department/resource   Subnet                Gateway            Representative
                                                                                device
  10             CR1                   192.168.51.0/27     192.168.51.1     CR1-PC
                                                                                192.168.51.2
  20             CR2                   192.168.51.32/27    192.168.51.33    CR2-PC
                                                                                192.168.51.34
  30             CR3                   192.168.51.64/27    192.168.51.65    CR3-PC
                                                                                192.168.51.66
  40             CR4                   192.168.51.96/27    192.168.51.97    CR4-PC
                                                                                192.168.51.98
  50             CR5                   192.168.51.128/27   192.168.51.129   CR5-PC
                                                                                192.168.51.130
  60             Shared printer        192.168.51.160/27   192.168.51.161   Printer
                                                                            192.168.51.162

Technologies
- Cisco Packet Tracer
- IPv4 addressing and subnetting
- VLANs
- IEEE 802.1Q trunking
- Router-on-a-Stick
- Static IP addressing
- ICMP ping testing
- ACLs, if implemented and verified in the final configuration

- Verification
The Phase 2 evidence report records successful ping tests from CR1-PC
(192.168.51.2) to its gateway (192.168.51.1), CR2 (192.168.51.34),
CR3 (192.168.51.66), CR4 (192.168.51.98), CR5 (192.168.51.130) and
the shared printer (192.168.51.162).

Security requirements and verification status currently
To prevent direct file sharing between departments, access to the shared printer must be allowed. Inter-VLAN routing, when enabled, doesn't constrain this by itself.

Troubleshooting and learning
Verify VLAN membership, trunk status, IP address, subnet mask, default gateway, and router subinterface status if connectivity issues come up.
The project provides hands-on experience with subinterfaces, trunk links, VLANs, subnetting, and testing connectivity in a systematic way.

References
- North-West University. (2026). CMPG325 Computer Networks:
  Individual Semester Project Brief.
- Cisco Systems, Inc. (2025). Configure Inter-VLAN Routing with the
  Use of an External Router.


