# Hotel Network Infrastructure

Cisco Packet Tracer project demonstrating the design and configuration of a multi-floor hotel network infrastructure.

## Overview

The network represents a three-floor hotel infrastructure divided into three main LAN segments.

The topology consists of three routers (R1, R2 and R3), multiple Layer-2 switches, end devices and server infrastructure.

## Network Architecture

### LAN1 – Administrative Segment

- Administrative Office – `192.168.1.0/24`
- Marketing Department – `192.168.2.0/24`
- IT Department – `192.168.3.0/30`
- DHCP provided by R1
- Administrative workstation with static IP configuration
- Remaining client devices use DHCP

### LAN2 – Operational Segment

- Reception – `193.168.1.0/24`
- Second Floor – `193.168.2.0/24`
- DHCP provided by R1
- Static and dynamic addressing according to department requirements

### LAN3 – Server and Third Floor Segment

- Server Room – `194.168.1.0/24`
- Third Floor – `194.168.2.0/24`
- DHCP provided by R3
- Servers use static IP configuration

## Router Configuration

### R1

- `FastEthernet0/0` – `192.168.1.1/24`
- `FastEthernet0/1` – `193.168.1.1/24`
- `Serial0/0/0` – `200.200.200.1/30`
- DHCP for LAN1 and LAN2 subnets

### R2

- `FastEthernet0/0` – `192.168.2.1/24`
- `FastEthernet0/1` – `193.168.2.1/24`
- `Serial0/0/0` – `200.200.200.2/30`
- `Serial0/0/1` – `200.200.201.1/30`

### R3

- `FastEthernet0/0` – `194.168.1.1/24`
- `FastEthernet0/1` – `194.168.2.1/24`
- `Serial0/0/1` – `200.200.201.2/30`
- DHCP for the Third Floor subnet

## Technologies

- Cisco Packet Tracer
- IPv4 addressing
- Subnetting
- DHCP
- Static IP configuration
- Dynamic IP configuration
- Router configuration
- Layer-2 switching
- Serial WAN links
- Multi-router network topology

## Project Objectives

The objective of this project was to design and configure a multi-segment hotel network with:

- Departmental network segmentation
- Static and dynamic IP addressing
- DHCP services
- Inter-router connectivity
- Dedicated server infrastructure
- Multiple LAN segments across three floors

## Files

- `hotel-network-infrastructure.pkt` – Cisco Packet Tracer topology and configuration