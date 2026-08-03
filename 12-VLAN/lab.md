# Lab 10 - VLAN Configuration

## Objective

Create VLANs and assign switch ports to different VLANs.

## Devices

- 1 Switch (2960)
- 2 PCs

## Topology

PC0 -------- Switch -------- PC1

## IP Addressing

PC0
192.168.10.10/24

PC1
192.168.20.10/24

## VLAN Configuration

VLAN 10 → SALES

VLAN 20 → IT

PC0 → Fa0/1 → VLAN 10

PC1 → Fa0/2 → VLAN 20

## Configuration

```bash
enable
configure terminal

vlan 10
name SALES
exit

vlan 20
name IT
exit

interface fa0/1
switchport mode access
switchport access vlan 10
exit

interface fa0/2
switchport mode access
switchport access vlan 20
exit

end
```

## Verification

```bash
show vlan brief
```

## Expected Result

- VLAN 10 created.
- VLAN 20 created.
- Ports assigned correctly.
