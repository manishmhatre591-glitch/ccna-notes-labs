# VLAN Configuration Commands

## Create VLAN 10

```bash
enable
configure terminal

vlan 10
name SALES
exit
```

## Create VLAN 20

```bash
vlan 20
name IT
exit
```

## Assign Port to VLAN 10

```bash
interface fastEthernet0/1
switchport mode access
switchport access vlan 10
exit
```

## Assign Port to VLAN 20

```bash
interface fastEthernet0/2
switchport mode access
switchport access vlan 20
exit
```

## Verification Commands

```bash
show vlan brief
show running-config
```
