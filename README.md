# Secure Enterprise Network Design (Packet Tracer Simulation)

## Project Overview

This project simulates the design and implementation of a scalable wired enterprise network using Cisco Packet Tracer. The objective was to design a structured IP addressing scheme using Fixed Length Subnet Masking (FLSM), configure routing between subnets, and enhance network security using Access Control Lists (ACLs) and port security.

The network was designed to support organizational growth over five years while maintaining performance, security, and structured segmentation.

---

## Network Requirements

The company required four subnets:

- Subnet A (LAN): 11 usable IP addresses
- Subnet B (LAN): 8 usable IP addresses
- Subnet C (WAN): 2 usable IP addresses
- Subnet D (LAN): 24 usable IP addresses

FLSM subnetting was implemented to ensure equal subnet sizes and simplified management.

---

## Network Architecture

<img width="1430" height="740" alt="image" src="https://github.com/user-attachments/assets/0cde161d-871e-4b55-9b87-8759579f0ac5" />


The network consists of:

- 2 Routers (R1 and R2)
- 4 Switches
- 4 PCs
- 1 extra PC to test features
- WAN connection between routers

The design enables full inter-subnet communication using static routing.

---

## Technical Implementation

### 1. Subnetting (FLSM)

- Calculated subnet ranges and masks

<img width="721" height="846" alt="image" src="https://github.com/user-attachments/assets/f12811b0-b781-4d1a-965c-011c9da40d58" />

  
- Assigned IP addresses systematically
- Ensured consistent subnet sizes across all networks

### 2. Router Configuration

- Configured Gigabit interfaces
- Assigned IP addresses
- Enabled serial WAN link
- Implemented static routing between subnets
- Verified using `ip route` and `ip int brief`

### 3. Connectivity Testing

- Ping tests between all PCs
- Traceroute validation
- Routing table verification

All devices successfully communicated across the network.

---

## Security Enhancements

### Standard Access Control List (ACL)

- Implemented standard ACL (1–99 range)
- Restricted access based on source IP address
- Applied ACL to router interfaces (inbound/outbound)

This ensured only authorized devices could access specific network segments.

### Port Security

- Configured access ports
- Limited MAC addresses per port
- Enabled sticky MAC feature
- Prevented unauthorized devices from connecting

This enhanced internal network security.

---

## Key Engineering Concepts Demonstrated

- IP subnetting (FLSM)
- Static routing
- WAN configuration
- Router CLI configuration
- Access Control Lists (ACL)
- Port security
- Network testing and troubleshooting
- Scalable infrastructure planning

---

## Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- Networking fundamentals (TCP/IP)

---

## Outcome

The final network successfully achieved:

- Full interconnectivity between all subnets
- Structured IP addressing
- Controlled access via ACL
- Device-level security through port security
- Expandable infrastructure design

This project demonstrates practical understanding of enterprise network architecture and applied network security principles, aligning with core Computer Engineering competencies.
