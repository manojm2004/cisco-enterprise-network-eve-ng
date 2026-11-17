# 🌐 Enterprise Multi-Department Network Simulation (EVE-NG)

A production-grade enterprise network topology simulated in **EVE-NG** using Cisco IOSv virtual routers and multilayer switches.

## 📌 Architecture Highlights
- **Hierarchical Network Design:** Core, Distribution, and Access layer separation.
- **VLAN Segmentation:** Dedicated VLANs for Engineering (VLAN 10), Finance (VLAN 20), HR (VLAN 30), and IT Operations (VLAN 99).
- **Inter-VLAN Routing:** Router-on-a-Stick via 802.1Q sub-interfaces and SVI configuration on multilayer switches.
- **Routing Protocol:** Single-Area **OSPFv2 (Area 0)** with dynamic route convergence, cost tuning, and passive interfaces.
- **Traffic Control:** Standard and Extended **Access Control Lists (ACLs)** restricting untrusted cross-department access to sensitive finance servers.
- **Address Management:** Cisco IOS DHCP Server pools with lease reservations and default gateway options.

## 📁 Repository Structure
- `configs/core_router.cfg`: Complete running configuration for Core Router R1 (OSPF, DHCP pools, Sub-interfaces).
- `configs/dist_switch.cfg`: SVI, VTP, and Spanning-Tree (Rapid-PVST) configuration.
- `configs/access_switch.cfg`: Access port security, 802.1Q trunking, and BPDU guard.

---
*Created by Manoj M | Network & Security Engineer*
