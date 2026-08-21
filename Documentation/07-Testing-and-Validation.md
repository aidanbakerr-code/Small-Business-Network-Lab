# Testing and Validation

## Overview

Testing was performed throughout the implementation process to verify that the network was operating as designed.

Testing covered:

- VLAN configuration
- Trunking
- Router-on-a-Stick
- DHCP
- DNS
- Inter-VLAN routing
- SSH
- Port Security
- Guest network isolation
- NAT/PAT
- Internet connectivity

---

## Testing Methodology

Testing was performed using a combination of:

- Cisco IOS verification commands
- Ping tests
- Client IP configuration checks
- DHCP lease verification
- NAT translation verification
- ACL verification
- Port Security verification
- End-to-end connectivity tests

The objective was to verify both **functionality** and **security**.

---

# 1. VLAN Testing

The VLAN configuration was verified on BDS-SW1 using:

show vlan brief
