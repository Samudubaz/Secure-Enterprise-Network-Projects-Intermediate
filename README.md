# Secure Enterprise Network Projects - Intermediate

This repository contains a collection of intermediate-level networking and security projects focusing on secure network design, firewall implementation, and intrusion prevention. These projects were developed in lab environments (Cisco Packet Tracer / FortiGate) to demonstrate practical networking concepts, with an emphasis on security, redundancy, and scalability.

## I. Project Strategy & Core Objectives
The primary goal of these projects is to explore and implement robust security architectures in enterprise-scale environments. Each project focuses on specific security layers:
*   **Security Zones:** Implementation of granular control through ZPF and segmentation.
*   **Traffic Inspection:** Deployment of IPS for real-time threat detection.
*   **Secure Connectivity:** Establishing encrypted communication channels via IPsec VPN.
*   **Policy Management:** Configuring high-performance firewall rules on FortiGate hardware.

---

## II. Individual Project Breakdowns

### 1. Secure Network Design Using Zone-Based Firewall (ZPF)
Implementation of a Zone-Based Policy Firewall (ZPF) using Cisco IOS to replace the traditional ACL-based stateful inspection.

#### Network Topology
![Network Topology](./1.Secure%20Network%20Design%20Using%20Zone-Based%20Firewall%20(ZPF)/Network%20Topology.png)

#### Implementation Details:
*   **Zones Configuration:** Defined Inside, Outside, and DMZ zones to facilitate strict traffic control.
*   **Policy Framework:** Used Class Maps to identify traffic, Policy Maps to define actions (inspect, drop, pass), and Service Policies to apply these to zone pairs.
*   **Key Security Task:** Ensuring the DMZ is accessible for web services while protecting the internal private network.

[ **[ Browse Files ]** ](./1.Secure%20Network%20Design%20Using%20Zone-Based%20Firewall%20(ZPF)/)

---

### 2. Cisco IOS-Based Intrusion Prevention System (IPS)
Configuration and deployment of a signature-based Intrusion Prevention System on Cisco perimeter routers.

#### Network Topology
![Network Topology](./2.Cisco%20IOS-Based%20Intrusion%20Prevention%20System%20(IPS)%20Configuration%20and%20Deployment/Network%20Topology.png)

#### Implementation Details:
*   **IPS Engine:** Configured Cisco IOS IPS to monitor traffic and take automated actions based on signature matches.
*   **Deployment:** Applied IPS rules on ingress/egress interfaces to mitigate threats at the network edge.
*   **Evidence:** Includes standard router configurations and Packet Tracer (PKT) files.

[ **[ Browse Files ]** ](./2.Cisco%20IOS-Based%20Intrusion%20Prevention%20System%20(IPS)%20Configuration%20and%20Deployment/)

---

### 3. IPsec-Based Secure Network Design
Designing a secure site-to-site communication channel across untrusted ISP networks using IPsec VPN.

#### Network Topology
![Network Topology](./3.IPsec-Based%20Secure%20Network%20Design%20with%20Advanced%20Security%20Features/Network%20Topology.png)

#### Implementation Details:
*   **Tunneling Strategy:** Implementation of GRE/IPsec for encrypted transport.
*   **ISAKMP Phase 1 & 2:** Precise configuration of encryption algorithms (AES), hashing (SHA), and authentication methods.
*   **Redundancy:** Simulated cross-ISP connectivity to ensure high availability for the VPN tunnel.

[ **[ Browse Files ]** ](./3.IPsec-Based%20Secure%20Network%20Design%20with%20Advanced%20Security%20Features/)

---

### 4. FortiGate Firewall Policy Implementation
Advanced network segmentation and security policy management using a FortiGate Firewall environment.

#### Network Topology
![Network Topology](./4.FortiGate-Based%20Firewall%20Policy%20Implementation%20with%20Network%20Segmentation/Network%20Topology.png)

#### Implementation Details:
*   **Segmentation:** Utilizing separate interfaces and VLANs for different department requirements.
*   **Security Profiles:** Implementation of Application Control, Web Filtering, and Antivirus profiles.
*   **RBAC:** Configuration of Administrator Roles to enforce the principle of least privilege.
*   **Interfaces & Policies:** Visual evidence provided via screenshots of the FortiOS dashboard.

[ **[ Browse Files ]** ](./4.FortiGate-Based%20Firewall%20Policy%20Implementation%20with%20Network%20Segmentation/)

---

## III. Tools & Technologies
*   **Cisco Packet Tracer:** For network simulation and configuration testing.
*   **FortiGate (FortiOS):** For next-generation firewall implementation.
*   **Cisco IOS:** Core routing and security platform.

---
*Developed for educational purposes and practical skill validation in Secure Network Infrastructure.*
