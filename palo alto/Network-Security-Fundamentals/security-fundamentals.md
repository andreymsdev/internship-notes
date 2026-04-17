# Navigating The Connected Globe

## Module Overview
This module explores how the globe is interconnected through network topologies, connectivity devices, routing protocols, and the Internet of Things (IoT).

---

## 1. The Evolution of the Internet
In the 1960s, the U.S. Defense Advanced Research Projects Agency (DARPA) created **ARPANET**, the precursor to the modern internet. It introduced **Packet Switching**, where data is broken into small packets and transmitted independently across the network to be reassembled at the destination.

The internet connects multiple **Local Area Networks (LANs)** into a worldwide **Wide Area Network (WAN)**. Today, billions of devices communicate using the **TCP/IP** standard over packet-switched networks.

---

## 2. Connectivity Devices

* **Routers:** Physical or virtual devices that forward data packets between networks using **logical addresses (IP)**. Routers determine the best path based on metrics like cost, delay, and distance.
* **Default Gateway:** The node that serves as an intermediary between your LAN and external networks (WAN/Internet). It handles traffic destined for addresses outside the local network.
* **Access Point (AP):** Connects to a wired network and transmits a Wi-Fi signal. A **Wireless Repeater** can be used to rebroadcast this signal and extend the range.
* **Hub:** A legacy device that connects multiple devices on a LAN. It broadcasts data to **all** ports, which is inefficient and insecure.
* **Switches:** Intelligent devices that use **physical addresses (MAC)** to forward data only to the specific destination port. 
    * **VLANs:** Switches can logically segregate a network into Virtual LANs to limit broadcast domains and improve security.

---

## 3. Topologies

### LAN Topologies
* **Star Topology:** All devices connect to a central hub or switch. Most common in modern LANs.
* **Mesh Topology:** Devices are interconnected, providing high redundancy.
* *Note: Legacy topologies like Ring and Bus are rarely found in modern enterprise networks.*

### WAN Resources
Common WAN equipment includes access servers, firewalls, modems, routers, VPN gateways, and WAN switches.

---

## 4. Routing Protocols

### Static vs. Dynamic Routing
* **Static Routing:** Routes are manually configured by an administrator. If a link goes down, traffic cannot be rerouted automatically.
* **Dynamic Routing:** Protocols automatically learn new paths and determine the best route. The routing table is updated periodically.

### Network Convergence
Convergence is the state where all routers on a network have a consistent and updated view of the network topology.
* **During Convergence:** Routers are exchanging updates; traffic might be dropped or looped because the routing tables are not yet synchronized.
* **Converged:** All routers agree on the best paths. The network is stable.
* **Without Convergence:** The network is unreliable, and data may never reach its destination.

---

## 5. DNS (Domain Name System)
DNS translates human-readable domain names (e.g., `google.com`) into IP addresses.

### The DNS Hierarchy & Recursive Queries
If a DNS server is not **authoritative** for a domain, it performs a **Recursive Query** in this order:
1.  **Root Name Servers:** 13 logical networks worldwide that direct queries to TLD servers.
2.  **Top-Level Domain (TLD) Servers:** Handle extensions like `.com`, `.org`, `.net`.
3.  **Authoritative DNS Servers:** Provide the actual IP address for the specific domain (e.g., `example.com`).

### Essential DNS Record Types
* **A Record:** Maps a domain name to an **IPv4** address.
* **AAAA Record:** Maps a domain name to an **IPv6** address.
* **CNAME (Canonical Name):** Aliases one domain name to another (e.g., `www.example.com` to `example.com`).
* **MX (Mail Exchanger):** Directs email to the correct mail server.

---

## 6. Networking Models: OSI vs. TCP/IP

The **OSI Model** is a theoretical framework (7 layers), while the **TCP/IP Model** (4 layers) is the practical implementation used in the real world.

| OSI Layer | TCP/IP Layer | Key Protocols |
| :--- | :--- | :--- |
| Application, Presentation, Session | **Application** | HTTP, DNS, FTP, SMTP |
| Transport | **Transport** | TCP, UDP |
| Network | **Internet** | IP, ICMP, Routing Protocols |
| Data Link, Physical | **Network Access** | Ethernet, Wi-Fi, MAC Addresses |