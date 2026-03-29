🏢 Enterprise Office Network Simulation (GNS3)

📌 Overview

This project demonstrates the design and implementation of an enterprise-level network using GNS3.
It follows a core–edge architecture and integrates key networking concepts such as routing, NAT, DHCP, and firewall security using ACLs.

The goal is to simulate a real-world office network with secure access control and internet connectivity.

---

🏗️ Network Architecture

The topology consists of:

- 🔹 Core Router (CORE-RTR): Internal routing and firewall enforcement
- 🔹 Edge Router (EDGE-RTR): Internet access using NAT
- 🔹 Core Switch (CORE-SW): Connects office devices
- 🔹 Office Network: HR, IT, Finance systems
- 🔹 Admin Network: Secured subnet 🔐
- 🔹 Customer Network: DHCP-based external network 📡

---

🌐 IP Addressing

Network| Subnet
Core ↔ Edge| 10.0.0.0/24
Office| 192.168.10.0/24
Admin| 192.168.20.0/24
Customer| 192.168.50.0/24

---

⚙️ Key Features

- ✅ Static IP addressing for office devices
- 📡 DHCP automatic IP assignment for customer network
- 🌐 NAT configuration for internet access
- 🔁 Static routing between networks
- 🔐 Firewall implementation using extended ACL
- 🧩 Network segmentation for security

---

🔐 Security (Firewall Logic)

- ✔ Admin network has full access to all networks
- ❌ Office and customer networks are restricted from accessing admin
- 🛡️ Access control enforced using extended ACL on the core router

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

Unauthorized access to the admin network is blocked.

"Firewall Block" (screenshots/firewall-block-test.png)
"Firewall Block HR" (screenshots/firewall-block-hr.png)

---

✅ Firewall – Allowed Access

Admin network can access all other networks.

"Firewall Allow" (screenshots/firewall-allow-test.png)

---

📡 DHCP Configuration

Customer devices receive IP automatically.

"DHCP" (screenshots/dhcp-auto-assignment.png)

---

🌐 Internet Access (NAT)

All devices can access the internet.

"Internet" (screenshots/internet-access-NAT.png)

---

🧰 Tools & Technologies

- 🖥️ Cisco 7200 Router (IOS)
- 🧪 GNS3 Network Simulator
- 💻 Oracle VM VirtualBox

---

📂 Project File

Due to file size limitations, the full GNS3 project is hosted externally:

🔗 https://drive.google.com/file/d/1mlkhLAarYJyHyTNzjELdpsSS7sZZXd11/view?usp=sharing

📁 Backup link available in:
"project-files/project-link.txt"

---

🎯 Key Learnings

- 📘 Enterprise network design principles
- 🌐 Practical implementation of NAT and routing
- 📡 DHCP configuration and management
- 🔐 Firewall security using ACL
- 🧩 Importance of network segmentation

---

📊 Summary

This project demonstrates a secure and scalable enterprise network design.
It integrates routing, NAT, DHCP, and firewall policies to ensure both connectivity and security in a real-world scenario.

---

👨‍💻 Author

Ananthu K Santhosh
BCA Student
Marian College Kuttikkanam

---
