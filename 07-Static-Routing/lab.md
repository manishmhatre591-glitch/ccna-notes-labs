# Lab 7 - Static Routing

## Objective

Configure static routing between two routers and verify end-to-end connectivity.

## Devices

- 2 Routers (2911)
- 2 PCs
- Copper Straight-Through Cables

## Topology

PC0 ---- R1 ---- R2 ---- PC1

## IP Addressing

### PC0

IP Address:
192.168.1.10

Subnet Mask:
255.255.255.0

Gateway:
192.168.1.1

### Router R1

G0/0
192.168.1.1/24

G0/1
10.0.0.1/30

### Router R2

G0/0
10.0.0.2/30

G0/1
192.168.2.1/24

### PC1

IP Address:
192.168.2.10

Subnet Mask:
255.255.255.0

Gateway:
192.168.2.1

## Steps

1. Build the topology.
2. Configure IP addresses on PCs.
3. Configure interfaces on R1 and R2.
4. Configure static routes.
5. Save the configuration.
6. Test connectivity using ping.

## Verification

From PC0:

ping 192.168.2.10

Expected Result:

Reply from 192.168.2.10
