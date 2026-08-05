# IP Addressing Plan

## Addressing Scheme

The network uses private IPv4 addressing with a separate /24 subnet allocated to each VLAN.

| VLAN | Department         | Network         | Default Gateway |
| ---- | ------------------ | --------------- | --------------- |
| 10   | Management         | 192.168.10.0/24 | 192.168.10.1    |
| 20   | IT                 | 192.168.20.0/24 | 192.168.20.1    |
| 30   | Finance            | 192.168.30.0/24 | 192.168.30.1    |
| 40   | Sales              | 192.168.40.0/24 | 192.168.40.1    |
| 50   | Marketing          | 192.168.50.0/24 | 192.168.50.1    |
| 60   | Support            | 192.168.60.0/24 | 192.168.60.1    |
| 70   | Administration     | 192.168.70.0/24 | 192.168.70.1    |
| 80   | Servers            | 192.168.80.0/24 | 192.168.80.1    |
| 90   | Guest Wi-Fi        | 192.168.90.0/24 | 192.168.90.1    |
| 99   | Network Management | 192.168.99.0/24 | 192.168.99.1    |

## Address Allocation

* Infrastructure devices use static IP addresses.
* Employee devices receive IP addresses through DHCP.
* Servers and printers use reserved static addresses.
* Additional address space has been reserved for future expansion.
