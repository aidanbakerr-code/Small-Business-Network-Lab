# VLAN Implementation

## Objective

VLANs were implemented to logically separate departments and network services.

This reduces unnecessary broadcast traffic and provides a foundation for network security.

---

## VLAN Configuration

| VLAN | Name | Assigned Ports |
|------|------|----------------|
| 10 | Management | Fa0/2 |
| 20 | IT | Fa0/3-4 |
| 30 | Finance | Fa0/5 |
| 40 | Sales | Fa0/6 |
| 50 | Marketing | Fa0/7 |
| 60 | Support | Fa0/8 |
| 70 | Administration | Fa0/9 |
| 80 | Servers | Fa0/10-11 |
| 90 | Guest Wi-Fi | Fa0/12 |
| 99 | Network Management | Fa0/13 |

---

## Trunk Configuration

Fa0/1 on BDS-SW1 operates as an 802.1Q trunk toward BDS-R1.

The trunk carries:

- VLAN 10
- VLAN 20
- VLAN 30
- VLAN 40
- VLAN 50
- VLAN 60
- VLAN 70
- VLAN 80
- VLAN 90
- VLAN 99

VLAN 99 is configured as the native VLAN.

---

## Verification

The configuration was verified using:

```text
show vlan brief
show interfaces trunk
