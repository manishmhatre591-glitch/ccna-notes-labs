# Lab 4 - IPv4 Address Configuration

## Objective

Configure IPv4 addresses on two PCs and verify connectivity.

## Devices Required

- 2 PCs
- 1 Switch

## Topology

PC0 -------- Switch -------- PC1

## IP Configuration

PC0

IP Address : 192.168.1.10

Subnet Mask : 255.255.255.0

Gateway : 192.168.1.1

PC1

IP Address : 192.168.1.20

Subnet Mask : 255.255.255.0

Gateway : 192.168.1.1

## Steps

1. Open Cisco Packet Tracer.
2. Place one Switch (2960).
3. Place two PCs.
4. Connect using Copper Straight-Through cables.
5. Configure the IP addresses on both PCs.
6. Open Command Prompt on PC0.
7. Run:

ping 192.168.1.20

## Expected Result

Reply from 192.168.1.20

Connectivity Successful.
