# Lab 13 - Inter-VLAN Routing

## Objective

Configure Router-on-a-Stick to allow communication between VLAN 10 and VLAN 20.

## Devices

- 1 Router (2911)
- 1 Switch (2960)
- 2 PCs

## Topology

PC0 ---- Switch ---- Router
PC1 ----/

## IP Addressing

### VLAN 10

PC0

192.168.10.10/24

Gateway

192.168.10.1

### VLAN 20

PC1

192.168.20.10/24

Gateway

192.168.20.1

## Steps

1. Create VLAN 10 and VLAN 20.
2. Assign access ports.
3. Configure trunk port.
4. Configure router sub-interfaces.
5. Ping PC1 from PC0.

## Verification

```bash
show interfaces trunk
show ip interface brief
ping 192.168.20.10
```

## Expected Result

PC0 successfully communicates with PC1 through the router.
