# NAT and Internet Connectivity

## Overview

Network Address Translation (NAT) and Port Address Translation (PAT) were implemented on BDS-R1 to provide Internet connectivity for the internal private networks.

The router translates internal RFC1918 addresses to the public-facing WAN address before traffic is forwarded to the simulated ISP network.

---

## Network Architecture

The external network consists of BDS-R1, ISP-R1, and a simulated Internet web server.


Internal VLANs
     |
     v
  BDS-SW1
     |
     v
  BDS-R1
     |
     | NAT/PAT
     |
     v
  ISP-R1
     |
     v
Internet Server
198.51.100.10
