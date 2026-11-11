# PacketTracer
A simple network of a company using packet tracer.

                    +-----------------------+

                    |   Cisco 2911 Router   |
                    |  (DHCP & Inter-VLAN)  |
                    +-----------+-----------+
                                | Gig0/0 (Sub-interfaces .10 & .20)
                                |
                       [ 802.1Q Trunk Link ]
                                |
                                | Gig0/1
                    +-----------+-----------+

                    |   Cisco 2960 Switch   |
                    +--+-----+-----+-----+--+

                       |     |     |     |
           +-----------+     |     |     +-----------+

           | Fa0/1           |     |           Fa0/4 |
           |           Fa0/2 |     | Fa0/3           |
           v                 v     v                 v
      +---------+       +---------+ +---------+       +---------+

      | HR PC 1 |       | HR PC 2 | | IT PC 1 |       | IT PC 2 |
      +---------+       +---------+ +---------+       +---------+
      \___________________________/ \___________________________/
         VLAN 10 (192.168.10.0/24)     VLAN 20 (192.168.20.0/24)
         Gateway: 192.168.10.1         Gateway: 192.168.20.1



         # Small Office Network Simulation (Cisco Packet Tracer)

![Network Topology]

## Overview
A simulated two-department (**HR** and **IT**) office network built in **Cisco Packet Tracer**. It demonstrates VLAN segmentation, inter-VLAN routing, automated DHCP, and basic network security.

## Network Setup

| Department | VLAN | Subnet | Gateway | Switch Ports |
| :--- | :--- | :--- | :--- | :--- |
| **HR** | VLAN 10 | `192.168.10.0/24` | `192.168.10.1` | `Fa0/1 - Fa0/2` |
| **IT** | VLAN 20 | `192.168.20.0/24` | `192.168.20.1` | `Fa0/3 - Fa0/4` |

* **Hardware:** 1x Cisco 2911 Router, 1x Cisco 2960 Switch, 4x PCs.
* **Features:** Router-on-a-Stick (802.1Q trunking), DHCP pools, SSH remote access, and switch port security.

## How to Use
Download packet tracer to be able to use it.

