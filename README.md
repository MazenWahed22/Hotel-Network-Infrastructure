# Hotel-Network-Infrastructure
📘 README – Hotel Network Infrastructure Project
🏨 Project Overview

This project implements a complete network infrastructure for a hotel consisting of 3 floors. Each floor contains different departments, and each department is assigned its own VLAN to ensure proper segmentation and security.

Floor 1 → Reception, Store, Logistics (3 VLANs)

Floor 2 → Finance, HR, Sales/Marketing (3 VLANs)

Floor 3 → IT, Admin (2 VLANs)

Each floor is equipped with:

A router (handling inter-VLAN routing, DHCP, and OSPF)

A switch (for VLAN segmentation)

A wireless access point (for Wi-Fi coverage per floor)

The 3 routers are interconnected using serial DCE cables and configured with OSPF for dynamic routing. SSH is enabled on all routers for secure remote access.

🛠️ Features & Configurations
🔹 VLANs

Each department is assigned to a dedicated VLAN to separate broadcast domains and enhance security.

🔹 DHCP

Configured on each router to automatically assign IP addresses for devices in the respective VLANs.

🔹 OSPF

Used as the routing protocol between the routers, allowing automatic route exchange and scalability.

🔹 Wireless Networks

Each floor has a wireless network connected to the floor’s switch, providing wireless access within the VLANs.

🔹 SSH

Secure remote login (SSH) enabled on all routers with usernames and privilege levels.

📐 Network Topology (Summary)

3 Routers → One per floor, interconnected via serial links.

3 Switches → One per floor, managing VLANs for departments.

8 VLANs total (3 + 3 + 2).

Wireless Access Points on each floor.

OSPF Area 0 interconnecting all routers.

DHCP Pools per VLAN.

SSH Remote Access configured on routers.

💡 Use Case / Why This Project is Important

This project simulates a real-world enterprise network for a hotel. It can be applied in scenarios such as:

🏨 Hotels or Large Offices → Separate VLANs for departments (Finance, HR, IT, etc.) to improve security and performance.

🔐 Centralized Security → VLANs + OSPF ensure isolated traffic while maintaining interconnectivity via routing.

📶 Wi-Fi per Floor → Employees and guests have stable wireless access, mapped to proper VLANs.

🛠 Scalability & Manageability → With OSPF and DHCP, the network is easy to expand and manage.

👨‍💻 Remote Management → SSH allows administrators to securely manage routers from anywhere.

This project can serve as a case study or training lab for network engineers preparing for CCNA/CCNP, or as a blueprint for real-life hotel/enterprise infrastructure design.

🚀 Future Improvements

Add a firewall (ASA or Zone-Based Firewall) for security policies between VLANs.

Configure QoS to prioritize traffic (e.g., VoIP for Reception, Finance apps for accounting).

Implement redundancy (HSRP/VRRP) for high availability.

Extend network with WAN connection for Internet and VPN access.
