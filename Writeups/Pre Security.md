###### <h2>🏴 Pre Security</h2> 

> Writeups for TryHackMe <br />
> Author: Tanny Thanh Nguyen

<br />
<h2>📚 Table of Contents</h2>

\- [Room 1: Offensive Security Intro](#room-1-Offensive-Security-Intro)

\- [Room 2: Defensive Security Intro](#room-2-Defensive-Security-Intro)

\- [Room 3: Careers in Cyber](#room-3-Careers-in-Cyber)

\- [Room 4: What is Networking?](#room-4-What-is-Networking?)

\- [Room 5: Intro to LAN](#room-5-Intro-to-LAN)

\- [Room 6: OSI Model](#room-6-OSI-Model)

\- [Room 7: Packets & Frames](#room-7-Packets-&-Frames)

\- [Room 8: Extending Your Network](#room-8-Extending-Your-Network)

\- [Room 9: DNS in Detail](#room-9-DNS-in-Detail)

\- [Room 10: HTTP in Detail](#room-10-HTTP-in-Detail)

\- [Room 11: How Websites Work](#room-11-How-Websites-Work)

\- [Room 12: Putting it all together](#room-12-Putting-it-all-together)

\- [Room 13: Linux Fundamentals Part 1](#room-13-Linux-Fundamentals-Part-1)

\- [Room 14: Linux Fundamentals Part 2](#room-14-Linux-Fundamentals-Part-2)

\- [Room 15: Linux Fundamentals Part 3](#room-15-Linux-Fundamentals-Part-3)

\- [Room 16: Windows Fundamentals Part 1](#room-16-Windows-Fundamentals-Part-1)

\- [Room 17: Windows Fundamentals Part 2](#room-17-Windows-Fundamentals-Part-2)

\- [Room 18: Windows Fundamentals Part 3](#room-18-Windows-Fundamentals-Part-3)

\- [Room 19: ](#room-19-)


<br />
<h2>🧩🏴 Room 1: Offensive Security Intro</h2>

* <a href="https://tryhackme.com/room/offensivesecurityintro">TryHackMe Room</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: Linux, Enumeration, Web Exploitation

### 1️⃣ Task 1: What is Offensive Security?
\- involves breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access

### 2️⃣ Tasks 2: First Hack
\- Command:  `gobuster -u http://fakebank.thm -w wordlist.txt dir`
  
\- Explain:

      gobuster: to discover hidden directories | subdomains
      -u: target url
      -w: wordlist file - each word will be appended into url to scan subdomains

  
### 🚩 Flags:
- Task 1: `Offensive Security`
- Task 2: `BANK-HACKED`




<br />
<hr>

<h2> 🧩🏴 Room 2: Defensive Security Intro </h2>

* <a href="https://tryhackme.com/room/defensivesecurityintro">TryHackMe Room</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: Defensive mindset    



### 1️⃣ Task 1: Defensive Security Intro
\- Defensive security = blue teaming

### 2️⃣ Task 2: Responsibilites of Defensive Security
\- Key areas of defensive security: Monitoring & detecting, incident response, threat intelligence, vulnerability management, investigation & analysis
<br />
\- DS team: a mixture of roles & responsibilities including: SOC analyst, incident responder, security engineer & digital forensics. 

### 3️⃣ Task 3: Defensive Security in Practice
SOC: Security operation center, the frontline of proctecting network, systems, data in an organisation, operating 24/7, 365 a year & typical daily activities in SOC: 
\-reviewing alerts triggered by security tooling
\-investigating anomalies 
\-responding to incidents.
<br />
SIEMs system ~ defensive security radar (Security information & event management system): critical part of any organisation's defensive security or IT, Where data & info from security devices, systems, servers,... are collected, reviewed & analysed.

### 4️⃣ Task 4: Practical: Defend FakeBank
Task: Investigate a security attack: <br />
- Recommend actions:

	Block source IP address
	Review admin panel access logs
	Implement rate limiting
	Update WAF rules

### 🚩 Flags:

* Task 1: `Blue teaming`
* Task 2: `Aaliyah` 
* Task 3: `SOC`
* Task 4: `THM{FAKEBANK-SECURED}`


<br />
<hr>
<h2> 🧩🏴 Room 3: Careers in Cyber</h2>

* <a href="https://tryhackme.com/room/careersincyber">Careers in Cyber</a></li>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### Roles: 
\- Security engineer, incident responder, malware analyst, penetration tester, red teamer.
<br />
\- Career quiz: penetration Tester


<br />
<hr>
<h2> 🧩🏴 Room 4: What is Networking?</h2>

* <a href="https://tryhackme.com/room/whatisnetworking"> What is Networking?</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: What is Networking?
\- That's devices connected together

### 2️⃣ Task 2:  What is the Internet?
\- A giant public network is made up of many small networks <br />
\- It is invented by Tim Berners-Lee in 1989 (the creation of the World Wide Web)

### 3️⃣ Task 3: Identifying Devices on a Network
\- IP address (or Internet Protocol): 4 octets <br />
\- MAC (Media Access Control): a unique address at the factory for physical network interface or microchip board inside the device. It's twelve-character hexadecimal number. First six characters represent the company that made the network interface and the last six is a unique number.
<br />
\- 50 billion devices connected to Internet by 2021 & IPv4 (4.29 billion) shortage => new IPv6 (>340 trillion addresses) 


### 4️⃣ Task 4: Ping
\- Ping uses ICMP (Internet Control Message Protocol) packets to determine the performance of a connection between devices.


### 🚩 Flags:
* Task 1:`Network`
* Task 2:`Tim Berners-Lee`
* Task 3:
	\- `Internet Protocol`
	\- `Octet`
	\- `4`
	\- `Media Access Control`
	\- `THM{YOU_GOT_ON_TRYHACKME}`
* Task 4:
	\- `ICMP`
	\- `ping 10.10.10.10`
	\- `THM{I_PINGED_THE_SERVER}`




<br />
<hr>
<h2> 🧩🏴 Room 5: Intro to LAN </h2>

* <a href="https://tryhackme.com/room/introtolan">Intro to LAN</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: Introducing LAN Topologies
- Topology: the design or look of the network <br />
\- Star topology: devices connected to a central witch/hub, most commonly found because of reliability and scalability instead of the cost. <br />
\- Bus Topology: similar to the leaf off of a tree (device ~ leaf), can't handle large data, slow and bottlenecked <br />
\- Ring Topology (= token topology): Devices connected directly to each other to form a loop, less bottlenecks than bus topology but one cable is cut, whole network fail.
- Switch: connect multiple devices together by MAC address (4, 8, ..., 64 ports for devices to plug into). It keep track of what device is connected to which port to forward the received packets to the intended port, so reducing network traffic & more efficient than hub (send the packets to all ports).<br />
- Router: routing to connect networks by IP address. Switch is faster for LAN, but only routers can connect the networks.


### 2️⃣ Task 2:  A Primer on Subnetting
\- 

### 3️⃣ Task 3: ARP
ARP: to find MAC address in LAN, use broadcast (router prevents broadcast). 2 message types: <br />
\-  ARP Request:  "Who has 192.168.1.20? send MAC for me" <br />
\-  ARP Reply: "I'm 192.168.1.20 — my MAC: AA:BB:CC:DD:EE:FF” <br />
\-  Then they save IP & MAC address into ARP table. Any device has a cache to store ARP table.


### 4️⃣ Task 4: DHCP
DHCP (Dynamic Host Configuration Protocol) server

### 🚩 Flags:
* Task 1: `Local Area Network`
	\- `Routing`
	\- `Switch`
	\- `Bus Topology`
	\- `Star Topology`
	\- `THM{TOPOLOGY_FLAWS}`

* Task 2: `Subnetting`
	\- `32`
	\- `0-255`
	\- `Network Address`
	\- `Host Address`
	\- `Default Gateway`

* Task 3: `Address Resolution Protocol`
	\- `Request`
	\- `MAC Address`
	\- `IP Address`
* Task 4: `DHCP Discover`
	\- `DHCP Request`
	\- `DHCP ACK`


<br />
<hr>
<h2> 🧩🏴 Room 6: OSI Model</h2>

* <a href="https://tryhackme.com/room/osimodelzi"> OSI Model</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: What is the OSI Model?
- OSI model (or Open Systems Interconnection Model): provides a framework dictating how all networked devices will send, receive and interpret data.
- It's a model for data travelling between & through 7 layers, also calles as process of data encapsulation.

### 2️⃣ Task 2: Layer 1 - Physical
Devices use electrical signals to transfer data between each other in binary number system: 1 or 0 (Ethernet cables)

### 3️⃣ Task 3: Layer 2 - Data Link 
- Communicating in LAN, by MAC address which is unique set for Network Interface Card (NIC).
- Data tranmission by Frame

### 4️⃣ Task 4: Layer 3 - Network
- Responsible for routing & re-assembly of data takes place (from these small chunks to the larger chunk) 
- By the protocols: OSPF (Open Shortest Path First) and RIP (Routing Information Protocol) to ensure the most optimal route (short & fast) across a network. 
- IP address used in this layer.

### 5️⃣ Task 5: Layer 4 - Transport
Transmitting data across a network and it follows 2 different protocols: 
- TCP (Transmission Control Protocol): reliability and guarantee the accuracy of data, used for file sharing, internet browsing or sending an email. 
- UDP (User Datagram Protocol): doesn't care if data is received or not for streaming. 

<br /> E.g., Video meeting rooms

### 6️⃣ Task 6: Layer 5 - Session
Manage the conversations: 
- Responsible opening, closing a connection 
- Save the checkpoints (where data is lost) (can continue to download a file when the connection breaks or restore 
- Sessions are unique: data in a session cannot travel to another session, one session for communicating with one device or application only. 


### 7️⃣ Task 7: Layer 6 - Presentation
as translator
- SSL/TLS encryption (HTTPS) 
- Data Compression (MP3, JPEG) 
- ASCII <-> Unicode 

### 8️⃣ Task 8: Layer 7 - Application
GUI (graphic user interface), e.g., DNS, browesr, email client, ... FTP client



### 🚩 Flags:
* Task 1: `Open Systems Interconnection`
	\- `7`
	\- `encapsulation`
* Task 2: `Physical`
	\- `Binary`
	\- `Ethernet Cables`
* Task 3: `Data Link`
	\- `Network Interface Card`
* Task 4: `Network`
	\- `Y`
	\- `Open Shortest Path First`
	\- `Routing Information Protocol`
	\- `IP Addresses`
* Task 5: `Transport`
	\- `Transmission Control Protocol`
	\- `User Datagram Protocol`
	\- `TCP`
	\- `UDP`
	\- `TCP`
	\- `TCP`
	\- `UDP`
* Task 6: `Session`
	\- `Session`
* Task 7: `Presentation`
	\- `Translator`
* Task 8: `Application`
	\- `Graphical User Interface`
* Task 9: `THM{OSI_DUNGEON_ESCAPED}`

<br />
<hr>

<h2> 🧩🏴 Room 7: Packets & Frames</h2>

* <a href="https://tryhackme.com/room/osimodelzi">Packets & Frames</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: What are Packets and Frames
Layer 2 (data link):
- Frame: data when it does not have IP address
\- Header layer 2 (source MAC) <br />
\- Payload (data)<br />
\- Trailer FCS (Frame Check Sequence) <br />

Layer 3 (Internet)
- Frame: has IP address
\- Header layer 2 (MAC source address) <br />
\- Payload: [ Header layer 3 (source IP) && payload (data)] <br />
\- Trailer FCS (Frame Check Sequence) <br />


### 2️⃣ Task 2: TCP/IP (The Three-Way Handshake)
- TCP: the protocol guarantees that any data sent will be received on the other end & called as Three-way handshake
- Kinds of messages are sent in TCP:

\- SYN: initial packet sent from client, to initiate a connection <br />
\- SYN/ACK: responded packet from server to acknowledge the synchronisation attempt from the client. <br />
\- ACK: can be used by either the client or server to acknowledge that messages/packets have been successfully received <br />
\- DATA: data segments is sent  <br />
\- FIN: Packet to close connection safely <br />
\- RST: packet to ends all  commmunication (immediately closing)

- Any communication of TCP started with 3 handshake: SYN-SYN/ACK-ACK

### 3️⃣ Task 3: Practical - Handshake
SERVER
| Client | Message | Server |
|------|-------|-------|
| SYN  | ===> |         |
|      | <=== | SYN/ACK |
| ACK  | <=== |     |
| DATA | <=== |     |
|      | <=== | ACK |
| FIN/ACK | <=== |  |
|      | <=== | FIN/ACK |
|   ACK   | <=== |         |

### 4️⃣ Task 4: UDP/IP
- User Datagram Protocol (UDP) is a stateless protocol that doesn't require a constant connection between the two devices for data to be sent.
- Faster than TCP, doesn't care if the data is received or not, & not reserve a continuous connection on a device as TCP does
- used in video streaming or voice chat.

| Client | Message | Server |
|------|-------|-------|
| Request | ===> |          |
|      	  | <=== | Response |
|      	  | <=== | Response |
|      	  | <=== | Response |


### 5️⃣ Task 5: Ports 101 (Practical)
Some well-known ports:
- 101: DNS
- 22: SSH
- 21: FPT
- 80: HTTP
- 443: HTTPS

### 🚩 Flags:
* Task 1: `Packet` 
	\- `Frame`
	\- ``
* Task 2:  `checksum` 
	\- `SYN,SYN/ACK,ACK`
* Task 3:  `THM{TCP_CHATTER}` 
* Task 4:  `User Datagram Protocol` 
	\- `stateless`
	\- `TCP`
	\- `UDP`
* Task 5:  `THM{YOU_CONNECTED_TO_A_PORT}` 


<br />
<hr>
<h2> 🧩🏴 Room 0: </h2>

* <a href=""> </a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: 
-
### 2️⃣ Task 2: 
-
### 3️⃣ Task 3: 
-
### 4️⃣ Task 4: 
-
### 5️⃣ Task 5:
-
### 6️⃣ Task 6:
-
### 7️⃣ Task 7:
-
### 8️⃣ Task 8:
-
### 9️⃣ Task 9:
-
### 0️⃣ Task 0:
-

### 🚩 Flags:
* Task 1:
	\- ``
	\- ``
* Task 2:
* Task 3:
* Task 4:


### 📌 General Notes
-
-
-


---







