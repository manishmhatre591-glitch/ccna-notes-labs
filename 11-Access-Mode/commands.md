# Access Mode Configuration

## Configure Fa0/1 for VLAN 10

```bash
enable
configure terminal

interface fastEthernet0/1
switchport mode access
switchport access vlan 10

exit
```

## Configure Fa0/2 for VLAN 20

```bash
interface fastEthernet0/2
switchport mode access
switchport access vlan 20

exit
```

## Verification Commands

```bash
show vlan brief
show interfaces switchport
show running-config
```
