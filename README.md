
# Databridge Innovations Network Design Using Cisco Packet Tracer

A Cisco Packet Tracer project that demonstrates the design, configuration, and testing of a small office network for **Databridge Innovations**. The project includes inter-department communication, DHCP and DNS configuration, and the implementation of an **Access Control List (ACL)** to enforce network security between departments.

## Table of Contents
- Project Overview
- Network Topology
- Tools and Technologies
- Configuration Steps
- Results and Findings
- Author

## Project Overview

This project was developed to design and implement a secure small office network for **Databridge Innovations** using **Cisco Packet Tracer**. The network consists of three departments—**Admin**, **Sales**, and **HR**—connected through a central router.

The project demonstrates basic network configuration, IP addressing, DHCP and DNS services, device connectivity testing, and the application of an **ACL** to restrict communication between specific departments while allowing authorized network access.

## Network Topology

The network consists of:

- **1 Cisco 2911 Router** renamed **Databridge**
- **3 Cisco 2960 Switches**
  - Admin Department
  - Sales Department
  - HR Department
- **6 PCs** (2 per department)
- **1 Server** providing **DHCP** and **DNS** services

### IP Addressing

- **Admin Department:** `192.168.10.0/24`
- **Sales Department:** `192.168.20.0/24`
- **HR Department:** `192.168.30.0/24`

### Server Configuration

- **DHCP Server:** `192.168.10.2`
- **DNS Server:** `192.168.10.3`

### Network Behavior

- All departments communicate through the **Databridge** router.
- PCs receive IP addresses automatically from the **DHCP** server.
- DNS services provide hostname resolution.
- An **ACL** prevents the **HR** department from communicating with the **Admin** department while allowing **Sales** to access Admin resources.

## Tools and Technologies

- **Cisco Packet Tracer**
- **Cisco 2911 Router**
- **Cisco 2960 Switches**
- **Desktop PCs**
- **DHCP Server**
- **DNS Server**
- **Command Line Interface (CLI)**
- **IPv4 Addressing**
- **Access Control Lists (ACLs)**
- **Ethernet Straight-through Cables**
- **Automatic Ethernet Connections**
- `configure terminal`
- `hostname Databridge`
- `ipconfig`
- `ping`

## Configuration Steps

1. Create the network topology in **Cisco Packet Tracer**.
2. Add one **Cisco 2911 Router**, three **Cisco 2960 Switches**, one server, and six PCs.
3. Rename the router to **Databridge** using the command `hostname Databridge`.
4. Rename each switch according to its department.
5. Assign IP addresses to the router interfaces for each subnet.
6. Configure the **DHCP** server to assign IP addresses automatically.
7. Configure the **DNS** server for hostname resolution.
8. Connect all devices using the appropriate Ethernet cables.
9. Configure router and server settings using the **CLI**.
10. Verify interface configuration and DHCP operation.
11. Configure an **ACL** to deny traffic from the **HR** subnet (`192.168.30.0/24`) to the **Admin** subnet (`192.168.10.0/24`).
12. Allow normal communication from the **Sales** subnet to the **Admin** subnet.
13. Test connectivity using the `ping` command.
14. Verify that:
    - **Sales → Admin** communication is successful.
    - **HR → Admin** communication is blocked.

## Results and Findings

The project successfully demonstrated the implementation of a secure multi-department office network.

Key achievements include:

- **Successful network design** using Cisco Packet Tracer.
- **Automatic IP address assignment** through DHCP.
- **DNS configuration** for network name resolution.
- **Successful communication** between authorized departments.
- **ACL implementation** to restrict unauthorized network access.
- **Successful verification** of ACL functionality through `ping` tests.
- Improved understanding of **network segmentation**, **traffic filtering**, and **basic network security** using Cisco routers.

## Author

**Name:** Ayo Bal

**Module:** Introduction to Networking

**Assignment:** Network Design Using Cisco Packet Tracer

**Date Submitted:** June 2, 2026
