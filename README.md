# 🖧 Enterprise Network Design Project

## 📌 Overview

This project demonstrates the design and implementation of a scalable and secure enterprise network using Layer 2 switches, Layer 3 (multilayer) switches, and routers.

The network supports VLAN segmentation, dynamic routing, redundancy protocols, wireless access, and centralized services like DHCP and TFTP.

---

## 🏗️ Network Architecture

The network is composed of:

* 🔹 Multiple **Layer 2 Switches** (Access Layer)
* 🔹 Two **Layer 3 Switches** (Distribution/Core Layer)
* 🔹 Three **Routers** (WAN / External Connectivity)
* 🔹 **Wireless Access Point (WAP)**
* 🔹 **Server** (Testing & Services)

---

## 🌐 VLAN Design

| VLAN | Purpose      | Hosts |
| ---- | ------------ | ----- |
| 10   | Department A | 100   |
| 20   | Department B | 50    |
| 30   | Department C | 25    |
| 40   | Department D | 10    |
| 99   | Management   | Admin |

---

## ⚙️ Features Implemented

### 🔸 Layer 2 Configuration

* VLAN segmentation
* Basic switch configuration (Console, VTY, SSH, Telnet)
* Port Security (MAC limiting & sticky MAC)
* BPDU Guard for loop prevention

---

### 🔸 Layer 3 Configuration

* Inter-VLAN Routing using SVIs
* HSRP for gateway redundancy
* OSPF for dynamic routing
* EtherChannel for link aggregation

---

### 🔸 Routing (Routers)

* OSPF configuration across 3 routers
* Network advertisement
* End-to-end connectivity validation

---

### 🔸 Services

* ✅ DHCP (Dynamic IP assignment for clients)
* ✅ TFTP (Backup configurations & IOS images)
* ✅ HTTP Server (Connectivity testing)

---

### 🔸 Security

* Access Control Lists (ACLs):

  * Allow HTTP (Port 80)
  * Allow ICMP (Ping)
  * Deny other traffic
* SSH for secure remote access
* Port Security & BPDU Guard

---

## 🧪 Testing & Validation

* ✔️ Ping between VLANs (Inter-VLAN Routing)
* ✔️ Failover testing using HSRP
* ✔️ OSPF route propagation
* ✔️ HTTP access to server
* ✔️ DHCP IP assignment verification

---

## 📂 Project Structure

```
📁 Enterprise-Network-Project
 ├── configs/
 │    ├── L2-switches/
 │    ├── L3-switches/
 │    └── routers/
 ├── topology/
 │    └── network_diagram.pkt
 ├── server/
 │    └── configuration.txt
 └── README.md
```

---

## 🚀 How to Run

1. Open the project in **Cisco Packet Tracer**
2. Load the provided `.pkt` topology file
3. Apply configurations (if not preloaded)
4. Start simulation and test:

   * Ping between VLANs
   * Access HTTP server
   * Verify DHCP assignment

---

## 📸 Screenshots (Optional)

> Add screenshots of:
>
> * Network topology
> * VLAN configuration
> * Successful ping tests
> * HSRP failover

---

## 🎯 Learning Outcomes

* Understanding VLAN segmentation
* Configuring inter-VLAN routing
* Implementing redundancy with HSRP
* Using OSPF for dynamic routing
* Applying network security techniques
* Managing enterprise network services

---

## 👤 Author

**Hazem Hamdy**

---

## 📜 License

This project is for educational purposes only.
