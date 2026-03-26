📖 1\. Room Overview  
The **OSI Model** (Open Systems Interconnection) room on TryHackMe is a foundational lab that explains how data moves across a network. It breaks down the complex process of sending a message from one computer to another into **seven distinct layers**, each with its own specific job and protocols.   
---

🏗️ 2\. The 7 Layers of the OSI Model  
To make this clear for your portfolio, I have categorized the layers from the **Application** (closest to the user) down to the **Physical** (the actual hardware). 

🖥️ Layer 7: Application

* **Purpose:** The layer you interact with. It provides network services to your software.  
* **Protocols:** HTTP, FTP, SMTP, DNS. 

🎭 Layer 6: Presentation

* **Purpose:** The "Translator." It handles data formatting, encryption, and compression so the application can understand it.  
* **Example:** SSL/TLS encryption. 

🤝 Layer 5: Session

* **Purpose:** Manages the "conversation" between devices. It starts, maintains, and ends the connection. 

---

🚀 3\. The Data Transport Layers  
📦 Layer 4: Transport

* **Purpose:** Decides how data is sent.  
* **TCP:** Reliable and checks for errors (used for web browsing).  
* **UDP:** Fast but doesn't check for errors (used for video streaming). 

🗺️ Layer 3: Network

* **Purpose:** The "Router" layer. It handles logical addressing and finding the best path for data.  
* **Unit:** Packets.  
* **Key Tool:** IP Addresses. 

---

🔌 4\. The Hardware Layers

🔗 Layer 2: Data Link

* **Purpose:** Handles physical addressing. It makes sure data gets to the right hardware on the local network.  
* **Unit:** Frames.  
* **Key Tool:** MAC Addresses and Switches. 

⚡ Layer 1: Physical

* **Purpose:** The actual electrical signals, fiber optics, or radio waves.  
* **Unit:** Bits (0s and 1s).  
* **Hardware:** Cables, Hubs, and WiFi frequencies. 

---

🚩 5\. Lab Activity & Flags  
In this lab, I completed the interactive challenge to correctly order the layers and identify which protocols belong to which level.

ANSWERS:

*What does the “OSI” in “OSI Model” stand for?*

*Open Systems Interconnection*

*How many layers (in digits) does the OSI model have?*

*7*

*What is the key term for when pieces of information get added to data?*

*Encapsulation*

**Task 2: Layer 1 — Physical**

*What is the name of this Layer?*

*Physical*

*What is the name of the numbering system that is both 0’s and 1's?*

*Binary*

*What is the name of the cables that are used to connect devices?*

*Ethernet Cables*

**Task 3: Layer 2 — Data Link**

*What is the name of this Layer?*

*Data Link*

*What is the name of the piece of hardware that all networked devices come with?*

*Network Interface Card*

**Task 4: Layer 3 — Network**

*What is the name of this Layer?*

*Network*

*Will packets take the most optimal route across a network? (Y/N)*

*Y*

*What does the acronym “OSPF” stand for?*

*Open Shortest Path First*

*What does the acronym “RIP” stand for?*

*Routing Information Protocol*

*What type of addresses are dealt with at this layer?*

*IP Addresses*

**Task 5: Layer 4 — Transport**

*What is the name of this Layer?*

*Transport*

*What does TCP stand for?*

*Transmission Control Protocol*

*What does UDP stand for?*

*User Datagram Protocol*

*What protocol guarantees the accuracy of data?*

*TCP*

*What protocol doesn’t care if data is received or not by the other device?*

*UDP*

*What protocol would an application such as an email client use?*

*TCP*

*What protocol would an application that downloads files use?*

*TCP*

*What protocol would an application that streams video use?*

*UDP*

***Task 6:*** 

*What is the name of this layer?*

*Session*

*What is the technical term for when a connection is successfully established?*

*Session*

***Task 7: Layer 6 — Presentation***

*What is the name of this Layer?*

*Presentation*

*What is the main purpose that this Layer acts as?*

*Translator*

***Task 8: Layer 7 — Application***

*What is the name of this Layer?*

*Application*

*What is the technical term that is given to the name of the software that users interact with?*

*Graphical User Interface*

***Task 9: Practical — OSI Game***

*Step 1: Click View Site*

*![][image1]*

*Step 2: Complete the game*

*For this game, use the arrow keys on your keyboard to reach a door, and hit the space bar to enter it.*

*Physical*

*Data link*

*Network*

*Transport*

*Session*

*Presentation*

*Application*

*Congratulations, you just learnt the basics of the OSI Model.*

---

🎓 6\. Conclusion & Skills Gained  
By completing this module, I mastered:

* Identifying where **Network Troubles** occur based on the OSI layer.  
* Understanding the difference between **TCP and UDP** transport.  
* Recognizing how **Encapsulation** works as data moves down the layers. 

[image1]: <data:image/png;base64,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>