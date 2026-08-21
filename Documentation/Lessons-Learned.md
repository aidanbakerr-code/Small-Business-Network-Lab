# Lessons Learned

## Overview

This project was designed to simulate the implementation of a small-business network from initial design through configuration, security implementation, troubleshooting, testing, and documentation.

The lab provided practical experience with Cisco networking concepts and demonstrated how multiple technologies work together to deliver a functional business network.

---

# Technical Skills Developed

During the project, I gained practical experience with:

- Cisco IOS configuration
- VLAN creation and segmentation
- Access port configuration
- 802.1Q trunking
- Router-on-a-Stick
- Inter-VLAN routing
- DHCP
- DNS
- SSH
- Switch management
- Port Security
- Sticky MAC addresses
- Access Control Lists
- Guest network isolation
- NAT/PAT
- Static and default routing
- Network troubleshooting
- Packet Tracer
- Network documentation

---

# VLAN Segmentation

One of the key lessons from the project was the importance of network segmentation.

Rather than placing all devices into a single broadcast domain, the network was divided into logical VLANs based on department and function.

This provided:

- Smaller broadcast domains
- Better organization
- Improved security
- Easier troubleshooting
- A foundation for access control

The Guest Wi-Fi network was placed into a separate VLAN so that it could be isolated from internal business resources.

---

# Router-on-a-Stick

Implementing Router-on-a-Stick provided practical experience with 802.1Q tagging and router subinterfaces.

The key concept was understanding that the switch does not perform the routing between VLANs in this design.

Instead:

```text
Client
   |
   v
Access VLAN
   |
   v
Switch
   |
   | 802.1Q Trunk
   v
Router Subinterface
   |
   v
Other VLAN
