# Router R1

```bash
enable
configure terminal

router rip
version 2
no auto-summary

network 192.168.1.0
network 10.0.0.0

end
```

---

# Router R2

```bash
enable
configure terminal

router rip
version 2
no auto-summary

network 10.0.0.0
network 192.168.2.0

end
```

## Verification Commands

```bash
show ip route
show ip protocols
show running-config
```
