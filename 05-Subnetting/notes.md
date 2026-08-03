# Subnetting Notes

## What is Subnetting?
Subnetting divides a large network into smaller logical networks.

## IPv4 Address
IPv4 contains 32 bits divided into:
- Network portion
- Host portion

Example:

192.168.1.10/24

Network: 192.168.1.0
Host: 10

## CIDR Notation

| CIDR | Mask | Usable Hosts |
|------|------|--------------|
| /24 | 255.255.255.0 | 254 |
| /25 | 255.255.255.128 | 126 |
| /26 | 255.255.255.192 | 62 |
| /27 | 255.255.255.224 | 30 |
| /28 | 255.255.255.240 | 14 |
| /29 | 255.255.255.248 | 6 |
| /30 | 255.255.255.252 | 2 |

## Formulas

Hosts:
2^host bits - 2

Subnets:
2^borrowed bits
