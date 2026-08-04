# Lab 12 - Configure Trunk Port

## Objective

Configure trunking between two Cisco switches.

## Devices

- 2 Cisco 2960 Switches
- 2 PCs

## Topology

PC0 ---- SW1 ===== SW2 ---- PC1

===== Trunk Link =====

## VLANs

VLAN 10

VLAN 20

## Configuration

### Switch 1

```bash
enable
configure terminal

vlan 10
name SALES

vlan 20
name IT

interface fa0/24
switchport mode trunk

end
```

### Switch 2

```bash
enable
configure terminal

vlan 10
name SALES

vlan 20
name IT

interface fa0/24
switchport mode trunk

end
```

## Verification

```bash
show interfaces trunk

show vlan brief
```

## Expected Result

- Trunk link is UP.
- VLAN 10 and VLAN 20 traffic can pass between switches.
