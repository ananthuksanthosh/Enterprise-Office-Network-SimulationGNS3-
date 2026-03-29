🏢 Enterprise Office Network Simulation (GNS3)

A practical enterprise network simulation built using GNS3 and Cisco 7200 routers. This project demonstrates real-world networking concepts such as routing, NAT, DHCP, and firewall implementation using ACLs.

---

📌 Project Overview

This project simulates a small enterprise network with multiple departments and a customer network. It focuses on secure communication, controlled access, and internet connectivity.

---

🏗️ Network Architecture

- Core Router (CORE-RTR) – Internal routing and firewall enforcement
- Edge Router (EDGE-RTR) – Internet gateway with NAT configuration
- Core Switch (CORE-SW) – Connects internal office devices
- Office Network – HR, IT, Finance departments
- Admin Network – Secure subnet with restricted access
- Customer Network – DHCP-enabled network for external users

---

🌐 IP Addressing Scheme

## 🌐 IP Addressing Scheme

| Network            | Subnet              | Description                         |
|------------------|--------------------|-------------------------------------|
| Core ↔ Edge Link | 10.0.0.0/24        | Router-to-router communication      |
| Office Network   | 192.168.10.0/24    | HR, IT, Finance departments         |
| Admin Network    | 192.168.20.0/24    | Secure admin systems                |
| Customer Network | 192.168.50.0/24    | DHCP-based external users           |
🚪 Default Gateways

- Office Network: 192.168.10.1
- Admin Network: 192.168.20.1
- Customer Network: 192.168.50.1

---

⚙️ Features Implemented

- Static IP addressing for office devices
- DHCP configuration for customer network
- NAT for internet access
- Static routing between routers
- Firewall implementation using extended ACL
- Network segmentation for security

---

🔐 Security (Firewall Implementation)

Firewall functionality is implemented using extended Access Control Lists (ACLs) on the Core Router (Cisco 7200).

- Admin network has full access to all networks
- Office and customer networks are restricted from accessing admin network
- Unauthorized traffic is blocked using ACL rules
- ACL applied on router interfaces to control traffic flow

---

🧪 Verification & Testing

✅ Internal Communication

Office devices communicate successfully
Example: HR → IT → FIN

Screenshot: "network-working.png"

---

🚫 Firewall Block

Unauthorized access to admin is blocked

Screenshots:

- "firewall-block-test.png"
- "firewall-block-hr.png"

---

✅ Firewall Allow

Admin can access all networks

Screenshot: "firewall-allow-test.png"

---

🌍 Internet Access (NAT)

Devices can access external network (8.8.8.8)

Screenshot: "internet-access-NAT.png"

---

📡 DHCP Verification

Customer devices receive IP automatically

Screenshot: "dhcp-auto-assignment.png"

---

📁 Project Structure

enterprise-office-network-gns3/
├── configs/
├── project-file/
├── screenshots/
└── README.md

---

🔗 GNS3 Project File

👉 "Download Full GNS3 Project" (https://drive.google.com/file/d/1mlkhLAarYJyHyTNzjELdpsSS7sZZXd11/view?usp=sharing)

---

🚀 How to Run

1. Install GNS3 and VirtualBox
2. Import Cisco 7200 router image
3. Download the project file
4. Open project in GNS3
5. Start all devices
6. Test connectivity using ping commands

---

🛠️ Technologies Used

- GNS3 (Network Simulation)
- Cisco 7200 Router (Core, Edge, Firewall roles)
- VPCS (Virtual PCs)
- VirtualBox

---

🎯 Learning Outcomes

- Enterprise network design basics
- Routing and NAT implementation
- Firewall using ACL
- DHCP configuration and troubleshooting
- Network segmentation and security

---

👨‍💻 Author

Ananthu K Santhosh
BCA Student | Interested in Networking & Cybersecurity

---

⭐ Conclusion

This project demonstrates a secure enterprise network with controlled access and internet connectivity using real-world networking concepts. It reflects practical hands-on experience with networking tools and configurations.

---
