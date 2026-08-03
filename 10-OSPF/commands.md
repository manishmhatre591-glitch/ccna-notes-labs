# Router R1

```bash
enable
configure terminal

router ospf 1

network 192.168.1.0 0.0.0.255 area 0
network 10.0.0.0 0.0.0.3 area 0

end
```

---

# Router R2

```bash
enable
configure terminal

router ospf 1

network 10.0.0.0 0.0.0.3 area 0
network 192.168.2.0 0.0.0.255 area 0

end
```

## Verification Commands

```bash
show ip route
show ip ospf neighbor
show ip protocols
show ip ospf interface
```
