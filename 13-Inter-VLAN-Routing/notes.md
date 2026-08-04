# Inter-VLAN Routing Notes

## What is Inter-VLAN Routing?

Inter-VLAN Routing allows devices in different VLANs to communicate with each other.

Since VLANs are separate broadcast domains, a Layer 3 device (Router or Layer 3 Switch) is required for communication.

## Router-on-a-Stick

Router-on-a-Stick is a method where one physical router interface is divided into multiple sub-interfaces.

Each sub-interface is assigned to a different VLAN.

## Important Commands

- interface g0/0.10
- encapsulation dot1Q 10
- ip address
- no shutdown

## Advantages

- Easy to configure
- Cost-effective
- Supports multiple VLANs over one physical link
