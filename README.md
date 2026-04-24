# Enterprise Network Design with VLAN WiFi VoIP(Cisco Packet Tracer)
This project simulates a **real-world enterprise network infrastructure** using Cisco Packet Tracer.

It includes:
- VLAN segmentation (HR, IT, ADMIN)
- Inter-VLAN routing (Router-on-a-Stick)
- Wireless network (WiFi)
- VoIP (IP Phones)
- DHCP configuration
- Shared services (Server, Printer, )

The goal is to design, configure, and troubleshoot a secure and scalable network.


# Departments (VLANs)

| VLAN | Name   | Devices             | Network            |
|------|--------|---------------------|--------------------|
| 10   | HR     | 4 PCs               | 192.168.10.0/24    |
| 20   | IT     | 2 PCs               | 192.168.20.0/24    |
| 30   | ADMIN  | 1 PC                | 192.168.30.0/24    |
| 40   | WIFI   | Smartphones         | 192.168.40.0/24    |
| 50   | VOICE  | IP Phones           | 192.168.50.0/24    |
|      | serveur| serveur             | 192.168.10.40      |
|      |prinnter| printer             | 192.168.30.10      |



# Network Topology

- 1 Router (Inter-VLAN Routing + DHCP)
- 1 Switch (Cisco 2960)
- 7 PCs
- 3 IP Phones
- 1 Access Point (WiFi)
- 1 Server
- 1 Printer

# Key Features

# VLAN Segmentation
Each department is isolated using VLANs to improve security and organization.

# Inter-VLAN Routing
Configured using **Router-on-a-Stick** to allow communication between VLANs.

# DHCP Configuration
Automatic IP assignment for:
- PCs
- Phones
- WiFi devices

# Voice VLAN
IP Phones use a dedicated VLAN (VLAN 50) for voice traffic.

# Wireless Network
Access Point provides WiFi access via VLAN 40.

# Testing & Validation

The network was tested using:

- DHCP IP assignment verification
- `ping` between VLANs
- Phone network connectivity
- Device communication with server

Expected results:
- All devices receive correct IP addresses
- Inter-VLAN communication works
- Voice devices are isolated in VLAN 50

# Skills Demonstrated

- Network design and topology planning
- VLAN configuration (Cisco Switch)
- Inter-VLAN routing (Router)
- DHCP configuration
- VoIP fundamentals (Voice VLAN)
- Wireless network integration
- Network troubleshooting

# Challenges Faced

- DHCP not responding due to trunk misconfiguration
- Missing network interface (FastEthernet) on PCs
- Incorrect VLAN assignment on switch ports
- IP Phones not powering on (PoE issue)

# Tools Used

- Cisco Packet Tracer

