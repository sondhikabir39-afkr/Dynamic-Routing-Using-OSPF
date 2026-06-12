# OSPF 3-Router Lab | Cisco Packet Tracer

## Overview

This project demonstrates the configuration of **Open Shortest Path First (OSPF)** using **three Cisco routers** in Cisco Packet Tracer. OSPF is a dynamic routing protocol that allows routers to automatically exchange routing information and find the best path to remote networks.

## Topology

```
PC1 ---- R1 ---- R2 ---- R3 ---- PC2
```

## Objectives

* Configure IP addresses on router interfaces.
* Configure OSPF on all three routers.
* Establish OSPF neighbor relationships.
* Automatically exchange routing information.
* Verify end-to-end connectivity using the `ping` command.

## IP Addressing Example

| Device | Interface | IP Address         |
| ------ | --------- | --------------     |
| R1     | G0/0      | 10.0.0.1/8         |
| R1     | G0/1      | 192.168.1.254/24   |
| R2     | G0/0      | 10.0.0.5/8         |
| R2     | G0/1      | 192.168.0.1/24     |
| R3     | G0/0      | 192.168.0.2/24     |
| R3     | G0/1      | 192.168.4.1/24     |

## OSPF Configuration

OSPF Process ID: **1**

All routers are configured to advertise their directly connected networks using OSPF.

## Verification Commands

```
show ip ospf neighbor
show ip route
show ip interface brief
ping <destination-ip>
```

## Expected Result

* OSPF neighbors form successfully.
* Routes are learned dynamically.
* All routers can communicate with each other.
* PCs connected to different routers can successfully exchange packets.

## Skills Demonstrated

* Cisco IOS CLI
* Dynamic Routing (OSPF)
* Router Configuration
* IP Addressing and Subnetting
* Network Troubleshooting
* Packet Tracer Simulation

## Author

Created as part of my CCNA Networking Lab Practice to strengthen routing and network configuration skills.
