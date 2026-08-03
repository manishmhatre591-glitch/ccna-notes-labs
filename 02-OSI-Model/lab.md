# Lab 2 - Understanding the OSI Model

## Objective

Understand how data travels between two PCs using the OSI Model.

## Software Required

- Cisco Packet Tracer

## Devices Required

- 1 Switch (2960)
- 2 PCs

## Topology

PC0 -------- Switch -------- PC1

## IP Address Configuration

PC0
IP Address : 192.168.1.10
Subnet Mask: 255.255.255.0

PC1
IP Address : 192.168.1.20
Subnet Mask: 255.255.255.0

## Steps

1. Open Cisco Packet Tracer.
2. Place one 2960 Switch.
3. Place two PCs.
4. Connect PCs to the Switch using Copper Straight-Through cables.
5. Configure IP addresses on both PCs.
6. Switch to Simulation Mode.
7. Send a Simple PDU from PC0 to PC1.
8. Observe the packet as it moves through the network.

## Observation

- Layer 7 – Application creates the data.
- Layer 6 – Presentation formats the data.
- Layer 5 – Session manages the session.
- Layer 4 – Transport adds TCP/UDP information.
- Layer 3 – Network adds IP addresses.
- Layer 2 – Data Link adds MAC addresses.
- Layer 1 – Physical sends bits over the cable.

## Result

Successfully observed packet flow through the OSI Model using Packet Tracer.
