🏢 Enterprise Office Network Simulation (GNS3)

📌 Overview

This project demonstrates the design and implementation of an enterprise-level network using GNS3.
It follows a core–edge architecture and includes routing, NAT, DHCP, and firewall security using ACLs.

The network simulates a real-world office environment with secure access control and internet connectivity.

---

🏗️ Network Architecture

- 🔹 Core Router (CORE-RTR) – Internal routing & firewall
- 🔹 Edge Router (EDGE-RTR) – Internet access (NAT)
- 🔹 Core Switch (CORE-SW) – Office network connectivity
- 🔹 Office Network – HR, IT, Finance systems
- 🔹 Admin Network – Secure subnet
- 🔹 Customer Network – DHCP-based network

---

🌐 IP Addressing

Network| Subnet
Core ↔ Edge| 10.0.0.0/24
Office| 192.168.10.0/24
Admin| 192.168.20.0/24
Customer| 192.168.50.0/24

---

⚙️ Features

- Static IP configuration for office devices
- DHCP automatic IP assignment for customer network
- NAT for internet connectivity
- Static routing between routers
- Firewall using extended ACL
- Network segmentation

---

🔐 Security (Firewall Logic)

- Admin network has full access to all networks
- Office and customer networks cannot access admin
- Implemented using extended ACL on core router

---

🚀 How to Run

1. Install GNS3 and VirtualBox
2. Download the project file from the link below
3. Import the project into GNS3
4. Start all devices
5. Open VPCS terminals
6. Test connectivity using ping commands

---

⭐ Highlights

- Designed multi-network enterprise topology
- Implemented firewall using ACL
- Configured DHCP for dynamic IP allocation
- Enabled internet access using NAT
- Applied real-world network segmentation

---

🧪 Verification

🖥️ Network Topology

"Topology" (screenshots/topology.png)

---

🔁 Internal Communication

Devices within the office network communicate successfully.

"Network Working" (screenshots/network-working.png)

---

🚫 Firewall – Blocked Access

Unauthorized access to admin network is blocked.

"Firewall Block" (screenshots/firewall-block-test.png)
"Firewall Block HR" (screenshots/firewall-block-hr.png)

---

✅ Firewall – Allowed Access

Admin network can access all other networks.

"Firewall Allow" (screenshots/firewall-allow-test.png)

---

📡 DHCP Auto Assignment

Customer network receives IP automatically.

"DHCP" (screenshots/dhcp-auto-assignment.png)

---

🌐 Internet Access (NAT)

Devices can access external network (8.8.8.8).

"Internet" (screenshots/internet-access-NAT.png)

---

🧰 Tools & Technologies

- Cisco 7200 Router (IOS)
- GNS3 Network Simulator
- Oracle VM VirtualBox

---

📂 Project File

🔗 https://drive.google.com/file/d/1mlkhLAarYJyHyTNzjELdpsSS7sZZXd11/view?usp=sharing

---

🏢 Real-World Use Case

This project simulates a small enterprise where:

- Employees communicate internally
- Admin network is secured
- Customer network is isolated
- Internet access is controlled via edge router

---

👨‍💻 Author

Ananthu K Santhosh
BCA Student
Marian College Kuttikkanam

---
