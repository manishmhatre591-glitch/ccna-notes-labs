# Lab 6 - Basic Router Configuration

## Objective

Configure a Cisco router using basic IOS commands.

## Devices

- 1 Router (2911)
- 1 PC

## Topology

PC0 -------- Router

## IP Address

Router G0/0

192.168.1.1/24

PC0

192.168.1.10/24

Gateway

192.168.1.1

## Steps

1. Drag one Router (2911).
2. Drag one PC.
3. Connect using Copper Straight-Through cable.
4. Configure the router:

```bash
enable
configure terminal
hostname R1

interface g0/0
ip address 192.168.1.1 255.255.255.0
no shutdown

end

copy running-config startup-config
```

5. Configure the PC IP address.
6. Open the PC Command Prompt.
7. Run:

```bash
ping 192.168.1.1
```

## Expected Result

- Router interface is up.
- PC successfully pings the router.
