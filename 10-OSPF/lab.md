# Lab 9 - OSPF Configuration

## Objective

Configure OSPF Area 0 between two routers.

## Devices

- 2 Routers (2911)
- 2 PCs

## Topology

PC0 ---- R1 ---- R2 ---- PC1

## IP Addressing

### PC0

192.168.1.10/24

Gateway: 192.168.1.1

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

192.168.2.10/24

Gateway: 192.168.2.1

## Steps

1. Configure IP addresses.
2. Configure OSPF on both routers.
3. Verify OSPF neighbors.
4. Verify the routing table.
5. Ping PC1 from PC0.

## Verification

```bash
show ip ospf neighbor
show ip route
ping 192.168.2.10
```

## Expected Result

- OSPF neighbor relationship is established.
- Routes are learned automatically.
- PC0 successfully pings PC1.
