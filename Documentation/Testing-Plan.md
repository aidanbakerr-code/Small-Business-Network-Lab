# Testing Plan

## Objectives

The network will be tested after configuration to verify functionality, security, and reliability.

## Test Cases

| Test                                       | Expected Result |
| ------------------------------------------ | --------------- |
| PC receives DHCP address                   | Pass            |
| PC reaches default gateway                 | Pass            |
| PC accesses internet simulation            | Pass            |
| Devices communicate within permitted VLANs | Pass            |
| Inter-VLAN routing functions correctly     | Pass            |
| Printer reachable from authorised VLANs    | Pass            |
| File server accessible                     | Pass            |
| SSH access to router and switch successful | Pass            |
| Guest Wi-Fi isolated from internal network | Pass            |

## Validation

The following evidence will be included in the repository:

* Ping tests
* Traceroute results
* Cisco IOS command output
* Configuration files
* Packet Tracer screenshots
* Network diagrams
