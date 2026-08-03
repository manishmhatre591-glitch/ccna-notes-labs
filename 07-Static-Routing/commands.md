# Router R1

```bash
enable
configure terminal

hostname R1

interface g0/0
ip address 192.168.1.1 255.255.255.0
no shutdown

interface g0/1
ip address 10.0.0.1 255.255.255.252
no shutdown

ip route 192.168.2.0 255.255.255.0 10.0.0.2

end
copy running-config startup-config
```

---

# Router R2

```bash
enable
configure terminal

hostname R2

interface g0/0
ip address 10.0.0.2 255.255.255.252
no shutdown

interface g0/1
ip address 192.168.2.1 255.255.255.0
no shutdown

ip route 192.168.1.0 255.255.255.0 10.0.0.1

end
copy running-config startup-config
```

## Verification Commands

```bash
show ip route
show ip interface brief
ping 192.168.2.10
```
