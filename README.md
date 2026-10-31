# Coffee-Shop-Network-Infrastructure
Small Business Network Design using Cisco Packet Tracer | VLAN, DHCP, ACL, SSH and Inter-VLAN Routing
# Coffee Shop Network Infrastructure

## Project Overview
A small business network designed and implemented
using Cisco Packet Tracer as part of my CCNA
networking practical learning.

The network provides separate connectivity for:
- Management Office
- Point of Sale (POS)
- Guest Wi-Fi
- Network Management

## Network Topology

Cisco Router 2911
       |
    802.1Q Trunk
       |
Cisco Catalyst 3560
   |     |     |
 VLAN10 VLAN20 VLAN30
 Office  POS   Guest Wi-Fi

VLAN 99 - Network Management

## VLAN and IP Addressing

| VLAN | Department | Network |
|------|------------|---------|
| 10 | Management | 192.168.10.0/24 |
| 20 | POS | 192.168.20.0/24 |
| 30 | Guest Wi-Fi | 192.168.30.0/24 |
| 99 | Network Management | 192.168.99.0/24 |

## Technologies Implemented

- VLAN Configuration
- Access and Trunk Ports
- IEEE 802.1Q
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP Configuration
- Extended Access Control Lists (ACL)
- SSH Remote Management
- Static IP Addressing
- Guest Network Isolation

## Security

Guest Wi-Fi users are restricted from accessing:
- Management Office Network
- POS Network
- Network Management Network

ACLs are configured on the router to enforce
network segmentation.

## Verification

- Verified VLAN assignments
- Verified trunk connectivity
- Verified router subinterfaces
- Verified DHCP IP allocation
- Tested guest network isolation
- Verified SSH version 2

## Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI

## Project Status

Core internal network configuration completed.

NAT, ISP connectivity and port security are
planned as future improvements.

## Author

Dhananjay Patil

## Project File

Download and open CoffeeShop_Project.pkt
using Cisco Packet Tracer.
