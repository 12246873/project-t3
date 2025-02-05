4.1. Network Design

4.1.1. Design the Network: 

Network Design of the residence hall: 

![Design-network](./main/task4-1-1-Design-network.png)

Network Design of on-site management office

![Management_office](./main/task-4-1-1-Managementoffice.png)

Network Design of the organisation’s main office: 

![Main_office](./main/task4-1-1-Mainoffice.png)

Combine network:

![Combine-Network](./main/task4-1-1-Combine-Network.png)

Key design decisions: 


The Key design will consider as per the separation of the networks in which ensure about the logical separation of main office operations, on-site management office, and residence hall networks for security and performance (Wynekoop, Johnson and Finan, 2021). The scalability of the network define by the design that allows future expansion if the residence hall or main office grows. The security of the network is calculate by protect sensitive business and resident data, including network segmentation, firewalls, and secure authentication methods. The cost efficiency of the network us define by the help of balancing quality hardware with cost considerations. It can be manage by centralized network management tools (Cisa, 2024). 


WiFi design:

Coverage and Configuration:

WiFi Access Points (APs): Deployed in the dining area and recreation room for strong, seamless coverage.

Settings:

•	SSID: "Hall-WiFi" (secured with WPA3 encryption).
•	Frequency Bands: Dual-band (2.4 GHz and 5 GHz) for compatibility and performance.
•	Channel Management: Auto-optimization to reduce interference.
•	Maximum Devices: Configured to handle peak concurrent connections for 240 residents.

Address allocations:

Based on a student ID ending in 73

IP Range: 73.0.0.0/16 for the entire network.

•	Main Office: 73.1.0.0/24.
•	Residence Hall: 73.2.0.0/24.
•	On-Site Office: 73.3.0.0/24.

Static IP Assignments included the point which reserved for network devices such as routers, switches, and servers.

Dynamic Allocation included the point which DHCP servers manage IPs for workstations, resident devices, and IoT equipment (Wynekoop, Johnson and Finan, 2021).



List of recommended hardware with specification: 

Device	Name	Cost (AUD)

Main Office and On-Site Office

Routers	Cisco ISR 4331	3500
Switch	Cisco Catalyst 9200	1500
Servers	Dell PowerEdge	4000
Residence Hall:
WiFi Access Points	Ubiquiti UniFi 6 Long-Range	200/unit
Switches	TP-Link TL-SG2428P	400
CCTV System:	Hikvision DS-2CD2T85FWD-I8	200/camera
RFID System	HID iCLASS SE Readers	300/reader


4.1.2. IP addressing Requirements: 

Based on a student ID ending in 73

IP Range: 73.0.0.0/16 for the entire network.

•	Main Office: 73.1.0.0/24.
•	Residence Hall: 73.2.0.0/24.
•	On-Site Office: 73.3.0.0/24.

References: 

Cisa (2024). Securing Network Infrastructure Devices | CISA. [online] Cybersecurity and Infrastructure Security Agency CISA. Available at: https://www.cisa.gov/news-events/news/securing-network-infrastructure-devices [Accessed 4 Jan. 2025].

Wynekoop, J., Johnson, D. and Finan, J. (2021). Enterprise Network Design: How is It Done? IFIP advances in information and communication technology, [online] pp.87–93. doi:https://doi.org/10.1007/978-0-387-35489-7_7.


4.2 Cloud Services

Network design:

![cloudservice](./main/task-4-2-CloudService.png)







