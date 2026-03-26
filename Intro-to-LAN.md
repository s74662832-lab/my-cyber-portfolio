📖 1\. Room Overview  
The **Intro to LAN** module is a core component of the **Pre-Security** pathway which I have done. This lab explores how devices connect within a private network, the physical layouts (topologies) used in modern offices, and the critical protocols that allow devices to talk to each other and the internet.  
---

🏗️ 2\. Task 1: LAN Topologies  
In this task, we analyze how devices are physically and logically arranged. Understanding these layouts is crucial for identifying single points of failure in a network.  
📝 Key Definitions:

* **LAN (Local Area Network):** A private network connecting computers in a small area (home, office, school).  
* **The Router:** Connects the LAN to the wider internet (WAN).  
* **The Switch:** Connects multiple devices *inside* the LAN.

📐 Comparison of Topologies:

1. **Star Topology:** Devices connect to a central switch.

   *Advantage:* Most common; if one cable fails, only that device is affected.

2. **Bus Topology:** Devices connect to a single main cable (backbone).

   *Disadvantage:* If the backbone breaks, the **entire network** goes down.

   

3. **Ring Topology:** Data travels in a circle.

   *Disadvantage:* Difficult to troubleshoot; a single break kills the whole loop.

ANSWERS:

*What does LAN stand for?*  
*Local Area Network*

*What is the verb given to the job that Routers perform?*  
*Routing*

*What device is used to centrally connect multiple devices on the local network and transmit data to the correct location?*  
*Switch*

*What topology is cost-efficient to set up?*  
*Bus Topology*

*What topology is expensive to set up and maintain?*  
*Star Topology*

*Complete the interactive lab attached to this task. What is the flag given at the end?*  
**Flag Found:** `THM{TOPOLOGY_FLAWS}`  
---

🍰 3\. Task 2: A Primer on Subnetting  
Subnetting is the process of dividing a large network into smaller, more efficient segments.  
🛠️ Technical Breakdown:

* **IP Address:** A 32-bit logical address (e.g., `192.168.1.20`) assigned to every device.  
* **Subnet Mask:** Used to separate the **Network ID** from the **Host ID**. A common mask is `255.255.255.0`.  
* **Octets:** IP addresses are split into four sections (octets). Each octet ranges from `0` to `255`.  
* **Default Gateway:** The IP address of the router. It acts as the "exit door" for any data leaving the local network.

ANSWERS:

*What is the technical term for dividing a network up into smaller pieces?*  
*Subnetting*

*How many bits are in a subnet mask?*  
*32*

*What is the range of a section (octet) of a subnet mask?*  
*0–225*

*What address is used to identify the start of a network?*  
*Network Address*

*What address is used to identify devices within a network?*  
*Host Address*

*What is the name used to identify the device responsible for sending data to another network?*  
*Default Gateway*

---

🔍 4\. Task 3: The ARP Protocol  
The **Address Resolution Protocol (ARP)** allows a device to find the physical hardware address (**MAC Address**) of another device when it only knows the **IP Address**.  
🔄 The Communication Process:

1. **The Request:** Device A broadcasts a message: *"Who has IP 192.168.1.5? Send me your MAC\!"*  
2. **The Reply:** Device B (the owner of that IP) responds: *"That's me\! Here is my MAC: 00:0a:95:9d:68:16."*  
3. **The Cache:** Device A saves this in its **ARP Table** so it doesn't have to ask again.

ANSWERS:

*What does ARP stand for?*  
*Address Resolution Protocol*

*What category of ARP Packet asks a device whether or not it has a specific IP address?*  
*Request*

*What address is used as a physical identifier for a device on a network?*  
*MAC Address*

*What address is used as a logical identifier for a device on a network?*  
*IP Address*

---

⚡ 5\. Task 4: The DHCP Protocol  
The **Dynamic Host Configuration Protocol (DHCP)** is like a "lease" system that automatically assigns IP addresses to devices when they join a network.  
🟦 The DORA Process:

1. **D \- Discover:** The client shouts for a DHCP server.  
2. **O \- Offer:** The server offers an available IP.  
3. **R \- Request:** The client asks to officially use that IP.  
4. **A \- Acknowledge (ACK):** The server confirms and the device connects.

ANSWERS:

*What type of DHCP packet is used by a device to retrieve an IP address?*  
*DHCP Discover*

*What type of DHCP packet does a device send once it has been offered an IP address by the DHCP server?*  
*DHCP Request*

*Finally, what is the last DHCP packet that is sent to a device from a DHCP server?*  
*DHCP ACK*  
---

🎓 6\. Conclusion & Skills Gained  
Completing this lab has provided me a deep understanding of:

* Identifying vulnerabilities in different **Network Topologies**.  
* Understanding how **Routers and Switches** manage traffic.  
* Troubleshooting connectivity issues via **ARP and DHCP** logic.

---

