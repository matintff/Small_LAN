# Small_LAN
 Design and Implementation of a Small Local Area Network with VLAN and DHCP Project 
 Goal:The goal of this project was to design a local area network (LAN) for a hypothetical company with three departments: Sales, IT, and Management. VLANs were used to segregate traffic between departments, and DHCP was utilized for automatic IP address assignment to devices in each VLAN.
 Network Topology: 
 • Devices: 
 • 1 Router (Cisco 2911) 
 • 1 Switch (2950-24) 
 • 6 Computers (PC) 
 • 1 Server 
 • Connections: 
 • The router is connected to the switch via port GigabitEthernet0/0. 
 • All PCs and the server are connected to the switch using Straight-Through cables. Configurations Performed: 1. VLAN Configuration (on the Switch): 
 • VLAN 10 (Sales): Assigned to ports FastEthernet0/2 and FastEthernet0/3 
 • VLAN 20 (IT): Assigned to ports FastEthernet0/4 and FastEthernet0/5 
 • VLAN 30 (Management): Assigned to ports FastEthernet0/6, FastEthernet0/7, and FastEthernet0/8 (for the server) 
 2. Router Configuration: 
 • Sub-interfaces were created for each VLAN with the following gateway IP addresses: 
 • 192.168.10.1 for VLAN 10 (Sales) 
 • 192.168.20.1 for VLAN 20 (IT) 
 • 192.168.30.1 for VLAN 30 (Management) 
 • DHCP pools were configured on the router to assign IP addresses to devices in each VLAN. 
 3. Switch Configuration: 
 • Port FastEthernet0/1 was set as a Trunk port to allow communication between the switch and the router for multiple VLANs. Results: 
• All devices successfully received automatic IP addresses from the DHCP server. 
• Inter-VLAN communication was successfully tested by pinging devices across different VLANs and the server. 
Conclusion:
This project demonstrates my ability to design and implement a small LAN using VLANs for traffic segregation, DHCP for IP management, and Inter-VLAN Routing for communication between departments.
![Small_LAN](https://github.com/user-attachments/assets/7b22fa61-fe9d-4a58-b6ad-50affd765e6a)
