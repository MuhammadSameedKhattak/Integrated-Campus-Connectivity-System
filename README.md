# Integrated Campus Management & Connectivity System (Packet Tracer)

## 📌 Project Overview
Architected a highly resilient and scalable campus network. This project simulates a multi-department corporate environment, focusing on high availability, logical traffic separation, and optimized routing protocols.

## 🏗️ Topology & Architecture
![Campus Topology](https://github.com/MuhammadSameedKhattak/Integrated-Campus-Connectivity-System/blob/main/NetworkTopology.png?raw=true)
**Key Design Features:**
* **Access Layer:** End-user connectivity for Departments (IT, HR, Sales).
* **Distribution Layer:** High-speed switching and gateway redundancy.
* **Core Layer:** Optimized path selection for inter-departmental communication.

## ⚙️ Core Technologies Implemented
* **HSRP (Hot Standby Router Protocol):** Configured gateway redundancy to ensure zero downtime. If the primary distribution switch fails, the standby takes over in milliseconds.
* **VTP (VLAN Trunking Protocol):** Deployed a VTP Server/Client domain to automate VLAN database propagation across the entire switch fabric.
* **Inter-VLAN Routing:** Implemented 802.1Q trunking to allow secure, routed communication between isolated logical networks.
* **DTP & Port-Security:** Managed trunk negotiation and secured access ports against unauthorized MAC addresses.

## 📊 Proof of Concept
### Gateway Redundancy (HSRP)
![HSRP Proof](https://github.com/MuhammadSameedKhattak/Integrated-Campus-Connectivity-System/blob/main/validation/HSRP-Status.png?raw=true)
*Caption: Output of `show standby brief` confirming Active/Standby states for the virtual gateway.*

### VLAN Distribution (VTP)
![VTP Proof](https://github.com/MuhammadSameedKhattak/Integrated-Campus-Connectivity-System/blob/main/validation/VLAN-Inventory.png?raw=true)
*Caption: Validation of VLAN inventory and VTP propagation across access switches.*
