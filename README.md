🏢 Enterprise Office Network Simulation (GNS3)

📌 Overview

This project demonstrates the design and implementation of a secure enterprise office network using GNS3.
The network is built using a core–edge architecture and integrates essential networking concepts such as routing, NAT, DHCP, and firewall security using Access Control Lists (ACLs).

The objective of this project is to simulate a real-world enterprise environment with multiple departments, controlled access to sensitive resources, and internet connectivity.

---

🏗️ Network Architecture

The network consists of the following components:

- Core Router (CORE-RTR):
  Responsible for internal routing between networks and enforcing firewall policies using ACLs

- Edge Router (EDGE-RTR):
  Connects the internal network to the internet and performs Network Address Translation (NAT)

- Core Switch (CORE-SW):
  Provides Layer 2 connectivity for office devices

- Office Network:
  Includes HR, IT, and Finance departments using static IP addressing

- Admin Network:
  A protected subnet with restricted access from other networks

- Customer Network:
  A separate network that uses DHCP for automatic IP assignment

---

🌐 IP Addressing Scheme

Network| Subnet| Description
Core ↔ Edge| 10.0.0.0/24| Router-to-router communication
Office Network| 192.168.10.0/24| HR, IT, FIN departments
Admin Network| 192.168.20.0/24| Secure administrative systems
Customer Network| 192.168.50.0/24| DHCP-based external users

---

⚙️ Features Implemented

- Static IP configuration for internal office systems
- DHCP configuration for customer network
- NAT configuration for internet access
- Static routing between core and edge routers
- Firewall implementation using extended ACL
- Network segmentation for improved security

---

🔐 Security Implementation (Firewall)

An extended Access Control List (ACL) is configured on the core router to enforce security policies:

- Administrative systems are allowed to access all networks
- Office and customer networks are restricted from accessing the admin network
- ACL rules are applied on multiple interfaces to ensure complete protection

This ensures that sensitive administrative resources remain secure while maintaining overall network connectivity.

---

🔄 Data Flow Explanation

- Office Users:
  PC → Core Switch → Core Router → Edge Router → Internet

- Customer Users:
  Device → Switch → Edge Router → Internet

- Admin Users:
  Admin systems can communicate with all internal and external networks

---

🚀 How to Run the Project

1. Install GNS3 and Oracle VM VirtualBox
2. Download the project file from the link below
3. Import the project into GNS3
4. Start all network devices
5. Open VPCS terminals for each PC
6. Verify connectivity using ping commands

---

⭐ Key Highlights

- Designed a multi-network enterprise topology
- Implemented firewall security using ACL
- Configured DHCP for dynamic IP allocation
- Enabled internet access using NAT
- Applied network segmentation for access control

---

🧪 Verification (Screenshots Included)

The following test cases were performed to validate the network:

- Topology Verification:
  Confirms correct network design and connectivity

- Internal Communication:
  Successful communication between office devices

- Firewall Blocking:
  HR and IT users cannot access admin network

- Firewall Allowing:
  Admin can access all networks

- DHCP Validation:
  Customer devices receive IP automatically

- Internet Connectivity:
  Successful ping to external address (8.8.8.8)

All related screenshots are available in the "screenshots/" directory:

- topology.png
- network-working.png
- firewall-block-test.png
- firewall-block-hr.png
- firewall-allow-test.png
- dhcp-auto-assignment.png
- internet-access-NAT.png

---

🧰 Tools & Technologies Used

- Cisco 7200 Router (IOS)
- GNS3 Network Simulator
- Oracle VM VirtualBox

Networking Concepts:

- IP Addressing
- Static Routing
- NAT (Network Address Translation)
- DHCP (Dynamic Host Configuration Protocol)
- ACL (Access Control List)

---

📂 Project File

The complete GNS3 project file can be accessed here:

https://drive.google.com/file/d/1mlkhLAarYJyHyTNzjELdpsSS7sZZXd11/view?usp=sharing

---

🏢 Real-World Use Case

This project simulates a small enterprise network where:

- Employees communicate across departments
- Administrative systems are protected from unauthorized access
- Customers access limited network services
- Internet access is managed through an edge router

---

🎯 Learning Outcomes

- Understanding of enterprise network design principles
- Practical implementation of routing and NAT
- Configuration of DHCP services
- Application of firewall security using ACL
- Importance of network segmentation

---

🎓 Conclusion

This project demonstrates how a secure and scalable enterprise network can be designed using industry-standard networking concepts.
It integrates routing, NAT, DHCP, and access control mechanisms to ensure both connectivity and security.

---

👨‍💻 Author

Ananthu K Santhosh
Bachelor of Computer Applications (BCA)
Marian College Kuttikkanam

---
