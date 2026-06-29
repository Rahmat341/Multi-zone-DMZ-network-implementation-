# Multi-zone-DMZ-network-implementation-
A secure three-zone DMZ network designed and implemented using Cisco Packet Tracer with ACL-based traffic control.
# Secure Multi-Zone DMZ Network Design & Implementation

## Overview
Designed and implemented a three-tiered DMZ network architecture 
in Cisco Packet Tracer to simulate a secure enterprise environment.

## Tools Used
- Cisco Packet Tracer
- Cisco 2911 Router
- Cisco 2960-24TT Switches

## Network Zones
| Zone | Subnet          |
|------|-----------------|
| WAN  | 192.168.1.0/24  |
| DMZ  | 172.16.1.0/24   |
| LAN  | 10.0.1.0/24     |

## Security Policies (ACL Rules)
- Allow HTTP/HTTPS (80/443) from WAN to DMZ Web Server
- Allow SQL traffic (1433) from DMZ Web Server to LAN Database
- Deny all traffic from WAN to LAN
- Deny all traffic from DMZ to WAN

## Verification
- Connectivity tested via ping from WAN PC to DMZ server
- ACL confirmed using: show access-lists 100
- Direct WAN to LAN database access successfully blocked

## Outcome
Successfully enforced network segmentation — public users 
could access the web server while the database remained 
protected from direct external access.
