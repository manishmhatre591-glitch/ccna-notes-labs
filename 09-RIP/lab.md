# Lab 9 - RIP Version 2

## Objective

Configure RIP Version 2 between two routers.

## Devices

- 2 Routers (2911)
- 2 PCs

## Topology

PC0 ---- R1 ---- R2 ---- PC1

## IP Addressing

### PC0
IP: 192.168.1.10/24
Gateway: 192.168.1.1

### R1
G0/0: 192.168.1.1/24
G0/1: 10.0.0.1/30

### R2
G0/0: 10.0.0.2/30
G0/1: 192.168.2.1/24

### PC1
IP: 192.168.2.10/24
Gateway: 192.168.2.1

## Steps

1. Configure IP addresses.
2. Verify direct connectivity.
3. Configure RIP Version 2 on both routers.
4. Verify routes using:

```bash
show ip route
```

5. Ping from PC0 to PC1.

## Expected Result

PC0 successfully communicates with PC1 using RIP.
