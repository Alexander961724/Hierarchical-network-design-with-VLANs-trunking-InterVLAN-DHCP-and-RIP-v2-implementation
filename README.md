# Hierarchical-network-design-with-VLANs-trunking-InterVLAN-DHCP-and-RIP-v2-implementation
# 🌐 Network Infrastructure Project  
./Campus-Simulation-Project.png 

This project implements a **Hierarchical Network Model** with VLANs, trunking, InterVLAN routing, DHCP, and RIPv2.

## 🏗️ **Network Architecture**  
The network follows a **Core, Distribution, and Access layer** model:  
- **Core Layer** – High-speed backbone connections.  
- **Distribution Layer** – Layer 3 switches for InterVLAN routing.  
- **Access Layer** – VLAN segmentation and end-user connectivity.  

## ⚙️ **Key Features**  
✔️ VLAN segmentation across different departments.  
✔️ Trunking and InterVLAN routing using Layer 3 switches.  
✔️ Dynamic IP assignment via DHCP.  
✔️ RIPv2 configured for dynamic routing.  
✔️ Default route implemented for external connectivity.  

## 🛠️ **Issues and Solutions**  

### ❌ **ISSUE #1: APIPA Address on VLAN 60 Computers**  
- **Problem:** Computers in VLAN 60 were receiving APIPA (169.254.x.x) addresses.  
- **Cause:** VLAN 60 was missing in the Access Layer switch.  
- ✅ **Solution:** Added VLAN 60, rechecked DHCP, and clients received correct IPs.  

### ❌ **ISSUE #2: "Gateway of Last Resort is Not Set" & No InterVLAN Communication**  
- **Problem:** Devices couldn't communicate across VLANs, and no default gateway was set.  
- **Cause:** The Layer 3 switch and router lacked a default route.  
- ✅ **Solution:** Configured a default route to ensure proper packet forwarding.  

## 🚀 **Project Summary**  
This project successfully implements a structured network with proper VLAN segmentation, dynamic routing, and troubleshooting solutions for common networking issues.  

## 🔗 **How to Use This Project**  
1️⃣ Clone this repository.  
2️⃣ Open the `.pkt` file in **Cisco Packet Tracer (v8.x or higher)**.  
3️⃣ Analyze the network topology and configurations.  

