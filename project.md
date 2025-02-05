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

4.2.1 Cloud Server Cost Comparison\

Cloud Provider	Region	CPU & RAM	Storage	Estimated Cost (AUD/Year)

AWS EC2        	Sydney	2 vCPUs, 8GB RAM	100GB    SSD	$780
Azure VM	      Australia East	2 vCPUs, 8GB RAM	100GB   SSD	$820
Google Cloud	  Sydney	2 vCPUs, 8GB RAM	100GB SSD	$760

Explanation:

The comparison evaluates AWS, Azure, and Google Cloud for hosting the web server. The chosen configuration ensures balanced performance and cost-effectiveness. Google Cloud emerges as the most cost-efficient ($760 per year), making it the recommended choice. Sydney is selected for low-latency access.



4.2.2 Backup Solutions

Backup Type	Provider	Storage Capacity	Cost (AUD/Year)	Pros	Cons

Cloud Backup	AWS S3 Glacier	5TB	$300	Secure, scalable	Data retrieval delays

Cloud Backup	Google Coldline	5TB	$280	Low cost, fast access	Requires setup

NAS (On-Prem)	Synology RAID 5	5TB	$1200 (one-time)	Full control, high speed	Hardware failure risk

Explanation:

Comparing cloud and non-cloud backups, Google Cloud Coldline ($280/year) is the most cost-effective. Cloud options are secure but retrieval speed varies. NAS offers instant access but is costly upfront. Cloud backup is recommended due to low maintenance and scalability.


4.3 Security

4.3.1 Cyber Security Risk Assessment

Threat Category	Risk	Asset Type	Impact	Likelihood	Risk Level

Unauthorized Access	High	Resident Data	Severe	Likely	Critical
Data Breach	High	Financial Records	Severe	Possible	High
Phishing	Medium	Email System	Moderate	Likely	High
Ransomware	High	Local Servers	Severe	Possible	High

Explanation:

The primary risks involve unauthorized access, data breaches, and ransomware. Resident data is the most vulnerable, requiring immediate security measures. Implementing MFA, encryption, and strict access control reduces risk significantly.


4.3.2 Security Controls Implementation

Security Control	Implementation	Risk Reduction	Drawbacks

Encryption	AES-256 for resident and financial data	Prevents unauthorized data access	Requires processing power
MFA	For admin and financial system login	Reduces risk of password compromise	User inconvenience
Firewall	Hardware firewall at network perimeter	Blocks unauthorized traffic	Setup complexity

Explanation:

Encryption safeguards sensitive data, MFA strengthens authentication, and firewalls prevent external threats. While these measures improve security, they may impact user convenience and system performance.



4.4.1 Data Collection Concerns

Ethical Concern	Risk	Recommendation

Excessive Data Collection	Privacy invasion	Collect only necessary information
Staff Access to Data	Unauthorized use	Implement role-based access control
Data Retention	Legal & ethical issues	Define clear retention policies

Explanation:

Collecting minimal data reduces privacy risks. Staff should only access necessary data, and retention policies must comply with regulations. Being transparent about data usage promotes ethical compliance.

4.4.2 Security Camera Ethical Issues


Concern	Ethical Impact	Recommendation

Surveillance of Private Areas	Invasion of privacy	Install cameras only in public areas
Data Retention	Risk of misuse	Store footage securely, limit retention period
Resident Access	Privacy concerns	Restrict access to authorized personnel only

Explanation:

This also means security cameras can only be installed in public areas. Data retention needs to be minimal, and footage should only be accessible to certain people to avoid misuse.

5 Project Management

5.1 Project Plan

Task	Responsibility	Deadline

Network Design	Team A	Week 5
Security Implementation	Team B	Week 7
Cloud Cost Estimation	Team C	Week 6
Ethical & Legal Review	Team D	Week 8

Explanation:

A very well-structured project plan guarantees the timely completion of tasks. The division of responsibilities among teams also improves efficiency. Constant check-ins and reviews avoid delays.

Reflection:
This project was very enlightening for me in terms of designing a network infrastructure for a real estate business concerning how cloud services and security measures are to be integrated with ethical considerations. It involved the process of evaluating cloud providers, assessing backup strategies, and conducting a cybersecurity risk assessment good lesson learned here-from which my understanding of real-world IT challenges has considerably improved. Besides, issues of data collection and surveillance have opened my eyes wider to understand that both business needs and requirements on privacy and compliance need to be balanced. On the whole, this project reinforced network design and implementation which have comprehensive planning, risk management, and ethical decision-making. 


References:
Achar, S., 2019. Cloud-based System Design. International Journal of All Research Education and Scientific Methods (IJARESM), 7(8), pp.23-30. 
Adami, D., Martini, B., Sgambelluri, A., Donatini, L., Gharbaoui, M., Castoldi, P. and Giordano, S., 2017. An SDN orchestrator for cloud data center: System design and experimental evaluation. Transactions on Emerging Telecommunications Technologies, 28(11), p.e3172. 
Carvalho, G.H., Woungang, I., Anpalagan, A., Jaseemuddin, M. and Hossain, E., 2017. Intercloud and HetNet for mobile cloud computing in 5G systems: Design issues, challenges, and optimization. IEEE Network, 31(3), pp.80-89. 
Ouda, G.K. and Yas, Q.M., 2021, February. Design of cloud computing for educational centers using private cloud computing: a case study. In Journal of Physics: Conference Series (Vol. 1804, No. 1, p. 012119). IOP Publishing.  



