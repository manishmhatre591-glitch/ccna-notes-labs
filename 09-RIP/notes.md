# RIP Notes

## What is RIP?

RIP (Routing Information Protocol) is a dynamic routing protocol that uses hop count as its routing metric.

## Features

- Distance Vector Routing Protocol
- Maximum Hop Count = 15
- Hop Count 16 = Unreachable
- Sends updates every 30 seconds

## RIP Version 1

- Classful Routing
- Does not support VLSM

## RIP Version 2

- Classless Routing
- Supports VLSM
- Supports Authentication
- Multicast Updates (224.0.0.9)

## Advantages

- Easy to configure
- Suitable for small networks

## Disadvantages

- Slow convergence
- Not suitable for large networks
- Limited to 15 hops
