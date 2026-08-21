# Network Design

## Overview

This project implements a small-business network for an organization consisting of approximately seven employees across multiple departments.

The network was designed in Cisco Packet Tracer with a focus on:

- Network segmentation
- Inter-VLAN routing
- Centralized DHCP
- DNS resolution
- Secure network management
- Layer 2 security
- Guest network isolation
- NAT/PAT
- Internet connectivity
- Testing and validation

The design follows a hierarchical approach where the access layer connects end-user devices to the managed switch, while the router provides inter-VLAN routing and external connectivity.

---

## Network Topology

The network consists of:

- Cisco managed Layer 2 switch
- Cisco business router
- Simulated ISP router
- Wireless access point
- Network servers
- Network printer
- Employee workstations
- Simulated external web server

The Cisco switch provides VLAN segmentation while the router provides routing between VLANs.

---

## Network Flow

Internal users connect to BDS-SW1.

BDS-SW1 forwards VLAN traffic over an 802.1Q trunk to BDS-R1.

BDS-R1 provides:

- Default gateways
- Inter-VLAN routing
- DHCP
- ACL enforcement
- NAT/PAT
- External connectivity

Traffic destined for the simulated Internet is forwarded to ISP-R1.

---

## Addressing Scheme

| VLAN | Name | Network | Gateway |
|------|------|---------|---------|
| 10 | Management | 192.168.10.0/24 | 192.168.10.1 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 |
| 40 | Sales | 192.168.40.0/24 | 192.168.40.1 |
| 50 | Marketing | 192.168.50.0/24 | 192.168.50.1 |
| 60 | Support | 192.168.60.0/24 | 192.168.60.1 |
| 70 | Administration | 192.168.70.0/24 | 192.168.70.1 |
| 80 | Servers | 192.168.80.0/24 | 192.168.80.1 |
| 90 | Guest Wi-Fi | 192.168.90.0/24 | 192.168.90.1 |
| 99 | Network Management | 192.168.99.0/24 | 192.168.99.1 |

---

## External Network

The simulated ISP network uses:

- BDS-R1 WAN: `203.0.113.2`
- ISP-R1: `203.0.113.1`

The simulated external network uses:

- ISP-R1: `198.51.100.1`
- Internet Web Server: `198.51.100.10`

---

## Design Objectives

The network was designed to provide:

1. Departmental segmentation
2. Controlled inter-VLAN communication
3. Secure administrative access
4. Guest network isolation
5. Automated IP addressing
6. Internal DNS resolution
7. Internet access through NAT/PAT
8. Basic Layer 2 security
9. A scalable addressing structure
10. A documented and testable configuration
