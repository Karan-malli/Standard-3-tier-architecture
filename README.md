# Standard-3-tier-architecture
 (Core → Distribution/Core → Access → End devices)
# Enterprise Network Lab - CCNA/CCNP Practice

![Network Topology](image.png)

Project Overview

This repository contains configurations and documentation for an enterprise network lab built to practice and demonstrate various networking concepts. The lab simulates a real-world hierarchical network design with redundancy, high availability, and routing protocols.

Lab Environment

- **Platform:** EVE-NG / GNS3 / Cisco Packet Tracer
- **Router OS:** Cisco IOS
- **Switch OS:** Cisco IOS / IOS-XE

Network Topology

The lab consists of a **3-tier hierarchical network architecture**:

| Layer | Devices | Description |
|-------|---------|-------------|
| **Gateway** | HQ | Edge router connecting to external networks |
| **Core** | CORE2, CORE3 | Core layer switches providing high-speed backbone |
| **Access** | Access4, Access5 | Access layer switches connecting end devices |
| **End Devices** | PC6, PC7 | Linux workstations for testing connectivity |



## ✅ Implemented Features

### Currently Configured

- [x] **Port Channel (EtherChannel)**
  - LACP between CORE2 and CORE3
  - Interfaces: E1/3 and E1/4
  
- [x] **HSRP (Hot Standby Router Protocol)**
  - High availability gateway for VLANs
  - Active/Standby configuration on CORE switches
  
- [x] **OSPF (Open Shortest Path First)**
  - Dynamic routing protocol
  - Single area configuration
