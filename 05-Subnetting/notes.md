# Subnetting Notes

## What is Subnetting?

Subnetting is the process of dividing one large network into multiple smaller networks (subnets).

## Why do we use Subnetting?

- Reduces network traffic
- Improves security
- Better IP address management
- Reduces broadcast domains

## Important Terms

### Network ID
The first IP address of a subnet.

Example:
192.168.10.0

### Broadcast ID
The last IP address of a subnet.

Example:
192.168.10.255

### Host Range
The usable IP addresses between the Network ID and Broadcast ID.

Example:
192.168.10.1 to 192.168.10.254

## CIDR Examples

/24 = 255.255.255.0

/25 = 255.255.255.128

/26 = 255.255.255.192

/27 = 255.255.255.224

## Example

Network:
192.168.10.0/24

Network ID:
192.168.10.0

Broadcast:
192.168.10.255

Usable Hosts:
192.168.10.1 - 192.168.10.254

Total Hosts:
254
