# DHCP and DNS

## Overview

BDS-R1 provides centralized DHCP services for the internal client VLANs.

DHCP automatically assigns IP configuration to client devices, while the internal DNS server provides hostname resolution for network resources and the simulated external web server.

---

## DHCP Design

DHCP pools were configured on BDS-R1 for the following VLANs:

| VLAN | Name | Network | Default Gateway | DNS Server |
|---:|---|---|---|---|
| 10 | Management | 192.168.10.0/24 | 192.168.10.1 | 8.8.8.8 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 | 8.8.8.8 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 | 8.8.8.8 |
| 40 | Sales | 192.168.40.0/24 | 192.168.40.1 | 8.8.8.8 |
| 50 | Marketing | 192.168.50.0/24 | 192.168.50.1 | 8.8.8.8 |
| 60 | Support | 192.168.60.0/24 | 192.168.60.1 | 8.8.8.8 |
| 70 | Administration | 192.168.70.0/24 | 192.168.70.1 | 8.8.8.8 |
| 90 | Guest Wi-Fi | 192.168.90.0/24 | 192.168.90.1 | 8.8.8.8 |

---

## DHCP Exclusions

The first 20 addresses of each client subnet were excluded from DHCP.

For example:


ip dhcp excluded-address 192.168.20.1 192.168.20.20
