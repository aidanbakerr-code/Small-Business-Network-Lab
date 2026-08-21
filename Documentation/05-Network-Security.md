# Network Security

## Overview

Basic network security controls were implemented to protect the small-business network from unauthorized access and limit unnecessary communication between network segments.

The security design uses multiple layers of protection rather than relying on a single control.

Implemented controls include:

- VLAN segmentation
- Dedicated management VLAN
- SSH remote administration
- Port Security
- Sticky MAC addresses
- Disabled unused switch ports
- Guest network isolation
- Extended ACL
- NAT/PAT

---

## VLAN Segmentation

The network is divided into separate VLANs based on department and function.

This provides logical separation between:

- Management
- IT
- Finance
- Sales
- Marketing
- Support
- Administration
- Servers
- Guest Wi-Fi
- Network Management

VLAN segmentation reduces broadcast domains and provides a foundation for access control.

---

## Management VLAN

VLAN 99 is dedicated to network management.

The switch management SVI uses:

IP Address: 192.168.99.2
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.99.1
