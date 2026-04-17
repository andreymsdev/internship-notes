#  Networking: Must Remember

## 1. Devices & Addresses (Layer 2 vs. Layer 3)
* **Switch:** Works on **Layer 2**. Uses **MAC Addresses** (Physical). It creates a "map" of which device is on which port.
* **Router:** Works on **Layer 3**. Uses **IP Addresses** (Logical). It connects different networks and finds the best path.
* **Default Gateway:** It’s the "exit door" of your LAN. If the destination IP isn't local, send it here.

---

## 2. The "Smart" Hub (VLANs)
* **Segmentation:** Use **VLANs** to break one physical switch into multiple logical networks (e.g., Guest Wi-Fi vs. Finance Dept).
* **Security:** VLANs limit **Broadcast Domains**—basically, they stop network "noise" and potential attacks from spreading to everyone.

---

## 3. Routing: Manual vs. Automatic
* **Static:** You write the path. **Pros:** Secure, low CPU. **Cons:** If a link dies, the network dies (no failover).
* **Dynamic:** Routers "talk" to each other. **Pros:** Heals itself if a cable is cut. **Cons:** Higher CPU, needs **Convergence**.
* **Convergence:** The moment when **all** routers finally agree on the map. If they haven't converged, packets get lost.

---

## 4. DNS: The Internet's Phonebook
If you can't access a site by name but can by IP, the problem is **DNS**.
* **Recursive Query:** The process of asking the Root -> TLD -> Authoritative server.
* **A Record:** Points to **IPv4**.
* **AAAA Record:** Points to **IPv6**.
* **MX Record:** Points to the **Mail** server.
* **CNAME:** A nickname (Alias) for a site.

---

## 5. OSI vs. TCP/IP (The Quick Map)
* **Layer 7 (Application):** Where the user is (HTTP, DNS).
* **Layer 4 (Transport):** Reliability (**TCP**) vs. Speed (**UDP**).
* **Layer 3 (Network):** IP addresses and Routers.
* **Layer 2 (Data Link):** MAC addresses and Switches.
* **Layer 1 (Physical):** Cables, fiber, and radio waves.

---

## 6. Packet Switching (ARPANET Legacy)
* Data is broken into **Packets**. 
* Each packet can take a **different path** to the destination. 
* This is why the internet is resilient—if one city goes dark, the packets just go around it.