# Small Business Network Design — Cisco Packet Tracer

## Project Overview

This project involves configuring and troubleshooting a small-business network in Cisco Packet Tracer. The lab separates departments using VLANs and enables communication between different subnets through router-on-a-stick inter-VLAN routing.

## Technologies and Skills

- Cisco Packet Tracer
- VLAN configuration and access ports
- IEEE 802.1Q trunking
- Router-on-a-stick inter-VLAN routing
- IPv4 addressing and subnet masks
- DHCP configuration and default gateways
- Network connectivity testing and troubleshooting

## Network Segmentation

| VLAN | Department | Network | Default Gateway |
|---|---|---|---|
| 10 | HR | 192.168.10.0/24 | 192.168.10.1 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 |

## Network Configuration

- Configured departmental VLANs on Cisco switches.
- Assigned end-device switch ports to their appropriate VLANs.
- Configured 802.1Q trunk links between the switches and router.
- Configured router subinterfaces to provide inter-VLAN routing.
- Configured and checked IPv4 addressing, DHCP leases, subnet masks, and default gateways.
- Configured a static IP address for the network printer and its default gateway.

## Troubleshooting and Validation

During testing, I identified and resolved network connectivity issues by:

- Adding VLAN 30 to the allowed VLAN list on the relevant trunk links.
- Correcting switch access-port VLAN assignments.
- Renewing client DHCP leases and checking IP configurations.
- Configuring the printer's default gateway to enable communication across subnets.

### Verified Tests

- Successful connectivity tests between HR, IT, and Finance devices.
- Successful communication with the Finance VLAN gateway.
- Successful connectivity to the network printer from within the Finance VLAN and from HR.
- Verified trunk status and VLAN membership using Cisco IOS show commands.

## Project Files

- `Small_Business_Network_Design.pkt` — Packet Tracer lab file, if included in the repository.

## Learning Outcomes

This lab provided practical experience with VLAN segmentation, trunk configuration, inter-VLAN routing, DHCP troubleshooting, default gateways, and systematic network connectivity testing.

