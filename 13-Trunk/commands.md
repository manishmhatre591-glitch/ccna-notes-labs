# Trunk Configuration Commands

## Configure Fa0/24 as Trunk

```bash
enable
configure terminal

interface fastEthernet0/24

switchport mode trunk

exit
```

## Allow VLANs

```bash
interface fastEthernet0/24

switchport trunk allowed vlan 10,20

exit
```

## Verification Commands

```bash
show interfaces trunk

show vlan brief

show running-config
```
