# Router-on-a-Stick

## Overview

Router-on-a-Stick (ROAS) was implemented to provide inter-VLAN routing using a single physical router interface divided into multiple 802.1Q subinterfaces.

This allows devices in different VLANs to communicate through BDS-R1 while maintaining logical network segmentation on BDS-SW1.

---

## Network Architecture

The connection between the switch and router is:

BDS-SW1 Fa0/1
      |
      | 802.1Q Trunk
      |
BDS-R1 G0/0
      |
      +-- G0/0.10 → VLAN 10
      +-- G0/0.20 → VLAN 20
      +-- G0/0.30 → VLAN 30
      +-- G0/0.40 → VLAN 40
      +-- G0/0.50 → VLAN 50
      +-- G0/0.60 → VLAN 60
      +-- G0/0.70 → VLAN 70
      +-- G0/0.80 → VLAN 80
      +-- G0/0.90 → VLAN 90
      +-- G0/0.99 → VLAN 99
