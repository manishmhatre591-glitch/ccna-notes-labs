# Switch Configuration

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

interface fa0/24
switchport mode trunk

end
```

---

# Router Configuration

```bash
enable
configure terminal

interface g0/0
no shutdown

interface g0/0.10
encapsulation dot1Q 10
ip address 192.168.10.1 255.255.255.0

interface g0/0.20
encapsulation dot1Q 20
ip address 192.168.20.1 255.255.255.0

end
```

## Verification Commands

```bash
show ip interface brief
show running-config
show interfaces trunk
ping
```
