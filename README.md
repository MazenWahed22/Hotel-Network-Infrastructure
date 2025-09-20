# 🏨 Hotel Network Infrastructure

## 📘 Project Overview

This project implements a **complete network infrastructure** for a hotel consisting of **3 floors**. Each floor contains different departments, and each department is assigned its own **VLAN** to ensure proper segmentation and security.

* **Floor 1** → Reception, Store, Logistics *(3 VLANs)*
* **Floor 2** → Finance, HR, Sales/Marketing *(3 VLANs)*
* **Floor 3** → IT, Admin *(2 VLANs)*

Each floor includes:

* 🖧 **Router** → Handles inter-VLAN routing, DHCP, and OSPF
* 🔌 **Switch** → Provides VLAN segmentation
* 📡 **Wireless Access Point** → Ensures Wi-Fi coverage

The **3 routers** are interconnected via **serial DCE cables** and configured with **OSPF** for dynamic routing.
🔐 **SSH** is enabled on all routers for secure remote access.

---

## 🛠️ Features & Configurations

### 🔹 VLANs

* Dedicated VLAN for each department.

### 🔹 DHCP

* Configured on each router to assign IPs automatically per VLAN.

### 🔹 OSPF

* Dynamic routing protocol interconnecting all routers under **Area 0**.

### 🔹 Wireless Networks

* Wi-Fi per floor, mapped to VLANs for seamless integration.

### 🔹 SSH

* Secure remote access enabled with usernames and privilege levels.

---

## 📐 Network Topology (Summary)

* **3 Routers** → One per floor, interconnected via serial links.
* **3 Switches** → One per floor, managing VLANs.
* **8 VLANs total** ( 3 + 3 + 2 ).
* **Wireless Access Points** → One per floor.
* **OSPF Area 0** → Backbone interconnection.
* **DHCP Pools** per VLAN.
* **SSH Remote Access** enabled.

---

## 💡 Use Case / Why This Project Matters

This project simulates a **real-world enterprise network** for a hotel, but it can be adapted for other environments like large offices or campuses.

* 🏨 **Hotels / Enterprises** → Department-based VLANs for performance & security.
* 🔐 **Centralized Security** → VLANs + OSPF ensure isolated yet connected networks.
* 📶 **Wi-Fi per Floor** → Stable wireless mapped to VLANs.
* 🛠 **Scalability** → OSPF & DHCP make expansion simple.
* 👨‍💻 **Remote Management** → Secure router management via SSH.

---

## 📜 Author
**Mazen Wahed**  
- 💼 [LinkedIn Profile](https://www.linkedin.com/in/mazen-wahed-260826320)  
- 📧 mazenwahed538@gmail.com  





