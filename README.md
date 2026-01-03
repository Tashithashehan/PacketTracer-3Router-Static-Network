# PacketTracer-3Router-Static-Network

## Project Overview
This repository contains a Cisco Packet Tracer simulation of a multi-router network using **Static Routing**. The project demonstrates how to manually configure routing tables to enable communication between three geographically or logically separate LANs without using dynamic protocols (like OSPF or RIP).

## Topology Features
* **No VLANs:** Each LAN is a flat network connected to a dedicated router interface.
* **Static Routing:** All paths are manually defined using the `ip route` command.
* **Switch-and-Spoke Connectivity:** Three branch routers connected via a central switch.

## Configuration Highlights

### 1. Gateway Setup
Each LAN uses a specific gateway IP (e.g., `192.168.1.15`) assigned to the router's FastEthernet or GigabitEthernet interface.

### 2. Static Route Logic
To ensure full connectivity, each router was configured with "Next-Hop" instructions. For example, to reach LAN 3 from LAN 1, the traffic is manually directed to the central router's IP.

