# Student Accommodation Network Simulation Project
## 1. Introduction
The goal of this project was to simulate and better understand the network infrastructure of my student accommodation. As a networking student, I was curious about how the network manages over 20+ buildings and provides internet access to hundreds of students. This simulation aimed to propose a logical and practical design while addressing inefficiencies observed in the existing setup.


## 2. Investigation and Findings
Through observation and research:
•	I discovered that each building has a dedicated room with network switches.
•	Every room has an access point for Wi-Fi connectivity.
With these findings I went on to design the network in the following way

![alt text](https://github.com/Moeketsi-ThatITGuy/Network_Projects/blob/main/network.png)

                            

## 3. Network Design Explained

- 	VLAN Segmentation: Each building was assigned a unique VLAN to limit broadcast traffic and improve performance.
- 	Inter-VLAN Routing: A multilayer switch was configured to route traffic between VLANs.
- 	DHCP: The multilayer switch was also configured to allocate IP addresses dynamically within a specified range for each VLAN.
- 	Access Points with a Unified SSID: All access points were configured to broadcast a single SSID, allowing seamless roaming between them.

## 4 Configuration Highlights:
### Basic switch configuration setup:

![alt text](https://github.com/Moeketsi-ThatITGuy/Network_Projects/blob/main/basic%20config.png)

### Vlans for each building and configuring switched virtual interface(SVI):

![alt text](https://github.com/Moeketsi-ThatITGuy/Network_Projects/blob/main/SVI.png)

### DHCP pools for each VLAN:

![alt text](https://github.com/Moeketsi-ThatITGuy/Network_Projects/blob/main/DHCP.png)

## 5.Checking if the configuration were setup correctly

### Used the ipconfig to confirm if the DHCP configuration were setup correctly

![alt text](https://github.com/Moeketsi-ThatITGuy/Network_Projects/blob/main/ipconfig.png)

### Checked if the inter-vlan routing is working by pinging different vlans

![alt text](https://github.com/Moeketsi-ThatITGuy/Network_Projects/blob/main/ping.png)

## 6. Conclusion and Lessons Learned

This project provided valuable insights into real-world networking practices and their limitations. Designing a VLAN-based network showed how segmentation can improve performance and scalability. Additionally, I learned the importance of troubleshooting configuration issues and optimizing network infrastructure to meet user needs.



