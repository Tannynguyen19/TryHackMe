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

\- [Room 7: ](#room-7-)
\- [Room 8: ](#room-8-)
\- [Room 9: ](#room-9-)
\- [Room 10: ](#room-10-)


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
-
### 2️⃣ Task 2: Layer 1 - Physical
-
### 3️⃣ Task 3: Layer 2 - Data Link 
-
### 4️⃣ Task 4: Layer 3 - Network
-
### 5️⃣ Task 5: Layer 4 - Transport
-
### 6️⃣ Task 6: Layer 5 - Session
-
### 7️⃣ Task 7: Layer 6 - Presentation
-
### 8️⃣ Task 8: Layer 7 - Application
-
### 9️⃣ Task 9: Practical - OSI Game
-


### 🚩 Flags:
* Task 1:
	\- ``
	\- ``
* Task 2:
* Task 3:
* Task 4: 
* Task 5:
* Task 6:
* Task 7:
* Task 8:
* Task 9:



### 📌 General Notes
-
-
-


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







