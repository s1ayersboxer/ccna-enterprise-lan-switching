# CCNA Enterprise LAN Switching & Routing

Simulated multi-department enterprise campus network featuring VLAN Segmentation, 802.1Q trunking, and Inter-VLAN routing.

## Tools & Technologies
* **Simulation Platform:** Cisco Packet Tracer
* **Protocols & Standards:** IEEE 802.1Q, VLANs, Spanning Tree Protocol (STP), Inter-VLAN Routing (Router-on-a-Stick), Port Security
* **Documentation:** draw.io (Logical Topology)

## Repository Structure
- '/config/' - Raw Device CLI configuration backup (.txt)
- '/diagrams/' - Network topology visuals (.png / .drawio)
- '/labs/' - Source simulation file (.pkt)

## Architecture & Implemtnation Highlights
1. **VLAN Segmentation:** Configured distinct VLANs for Data, Voice, Management, and Guest Traffic to isolate broadcast doamins.
2. **Trunking & Security:** Implemented 802.1Q trunking between access switches and distribution layers, securing unused ports, and enabling Port Security to restrict MAC address learning.
3. **Inter-VLAN Routing:** Configured a Router-on-a-Stick architecture utilizing subinterfaces tagged with 802.1Q encapsulation to route traffic between isolated VLANs.

## Vertification Commands
Key IOS Verification commands used during testing:
* 'show vlan brief'
* 'show interfaces trunk'
* 'show spanning-tree'
* 'shot ip route'
