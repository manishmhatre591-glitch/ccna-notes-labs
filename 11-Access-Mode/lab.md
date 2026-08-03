# Lab 11 - Configure Access Ports

## Objective

Configure switch access ports for different VLANs.

## Devices

- 1 Switch (2960)
- 2 PCs

## Topology

PC0 ---- Fa0/1 ---- Switch ---- Fa0/2 ---- PC1

## VLAN Configuration

VLAN 10 → SALES

VLAN 20 → IT

## Configuration

```bash
enable
configure terminal

vlan 10
name SALES

vlan 20
name IT

interface fa0/1
switchport mode access
switchport access vlan 10

interface fa0/2
switchport mode access
switchport access vlan 20

end
```

## Verification

```bash
show vlan brief
show interfaces switchport
```

## Expected Result

- Fa0/1 is assigned to VLAN 10.
- Fa0/2 is assigned to VLAN 20.
