# Static Routing Notes

## What is Static Routing?

Static Routing is a manual method of configuring routes on a router.

The network administrator manually tells the router where to send packets.

## Advantages

- Simple
- Secure
- Low CPU Usage
- Easy for Small Networks

## Disadvantages

- Manual Configuration
- Not suitable for large networks
- Every route must be configured manually

## Syntax

ip route <Destination Network> <Subnet Mask> <Next-Hop IP>

Example

ip route 192.168.2.0 255.255.255.0 10.0.0.2
