###### <h2>🏴 Pre Security</h2> 

> Writeups for TryHackMe <br />
> Author: Tanny Thanh Nguyen <br />
> Profile: <a href="https://tryhackme.com/p/ngtanny19">TryHackMe Profile</a> 

<br />
<h2>📚 Table of Contents</h2>

\- [Room 1: Offensive Security Intro](#room-1)

\- [Room 2: Defensive Security Intro](#room-2)

\- [Room 3: Careers in Cyber](#room-3)

\- [Room 4: What is Networking?](#room-4)

\- [Room 5: Intro to LAN](#room-5)

\- [Room 6: OSI Model](#room-6)

\- [Room 7: Packets & Frames](#room-7)

\- [Room 8: Extending Your Network](#room-8)

\- [Room 9: DNS in Detail](#room-9)

\- [Room 10: HTTP in Detail](#room-10)

\- [Room 11: How Websites Work](#room-11)

\- [Room 12: Putting it all together](#room-12)

\- [Room 13: Linux Fundamentals Part 1](#room-13)

\- [Room 14: Linux Fundamentals Part 2](#room-14)

\- [Room 15: Linux Fundamentals Part 3](#room-15)

\- [Room 16: Windows Fundamentals Part 1](#room-16)

\- [Room 17: Windows Fundamentals Part 2](#room-17)

\- [Room 18: Windows Fundamentals Part 3](#room-18)

\- [Room 19: ](#room-19)


<br />
<h2 id="room-1">🧩🏴 Room 1: Offensive Security Intro</h2>

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

<h2 id="room-2"> 🧩🏴 Room 2: Defensive Security Intro </h2>

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
<h2 id="room-3"> 🧩🏴 Room 3: Careers in Cyber</h2>

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
<h2 id="room-4"> 🧩🏴 Room 4: What is Networking?</h2>

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
<h2 id="room-5"> 🧩🏴 Room 5: Intro to LAN </h2>

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
<h2 id="room-6"> 🧩🏴 Room 6: OSI Model</h2>

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

<h2 id="room-7"> 🧩🏴 Room 7: Packets & Frames</h2>

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
<h2 id="room-8"> 🧩🏴 Room 8: Extending Your Network</h2>

* <a href="https://tryhackme.com/room/extendingyournetwork"> Extending Your Network</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1:  Introduction to Port Forwarding
NAT Router prevents all connections from Internet to protect LAN.
Port Forwarding is technique of redirecting network traffic from one port with IP address to another port with different IP address. 

- Server on laptop: `192.168.1.10:80`
- Port Forwarding rule on router: `Public: 203.0.113.25:8080 ---> Private: 192.168.1.10:80`
- Client can access server: `http://203.0.113.25:8080`

### 2️⃣ Task 2:  Firewalls 101
Firewall: determining what traffic is allowed to enter and exit, 2 types of firewall.
- Stateless ( packet filtering): check soure & dest IP, port, protocol. Not check payload or data, fast & for small/family network
- Statefull: check entire connection, packets/data based on session, slow & for enterprise, corporate.

### 3️⃣ Task 3: Practical - Firewall
Configure the firewall, set firewall rule to prevent the packets of specific IP from reaching the web sever.

### 4️⃣ Task 4: VPN Basics
Virtual Private Network (VPN) is a technology that allows devices on separate networks to communicate securely by creating a dedicated path between each other over the Internet (known as a tunnel). Devices connected within this tunnel form their own private network.

- Networks in different geographical locations to be connected: can hide your real IP, website only see the VPN server's IP & its location.
- Offers privacy & anonimity: protect you on public wifi, data is encrypted
- 3 VPN technologies: PPP, PPTP & IPSec (use IP framework, stable, highly secure, commonly for corporate VPN, firewall)

### 5️⃣ Task 5: LAN Networking Devices
- Router: routing to connect networks, creating a path (by decide if shortest, most reliable or faster medium) between networks so data can travel between them, operate on layer 3.

- Switch: a means of connecting to multiple devices, operate on layer 2 or 3.
\- Switch on layer 2: connect mutiple devices on same network (LAN) <br />
\- Switch on layer 3: connect mutiple networks (VLAN1 192.168.1.1, VLAN2 192.168.2.1, a network to be virtually split up) <br />


### 🚩 Flags:
* Task 1: `router`
* Task 2: `3 & 4`
	\- `stateful`
	\- `stateless`
* Task 3: `THM{FIREWALLS_RULE}`

* Task 4: `PPP`
	\- `IPSec`
* Task 5: `routing`
	\- `Layer 2,Layer 3`
* Task 6: `THM{YOU'VE_GOT_DATA}`
	\- `5`

<br />
<hr>
<h2 id="room-9"> 🧩🏴 Room 9: DNS in Detail</h2>

* <a href="https://tryhackme.com/room/dnsindetail"> DNS in Detail</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: What is DNS?
DNS (Domain Name System) provides a simple name for complex IP address

### 2️⃣ Task 2: Domain Hierarchy
- abc.com <br />
.: root domain <br />
abc: TLD (Top-Level Domain), 2 types of TLD: gTLD (Generic Top Level) & ccTLD (Country Code Top Level Domain, e.g., ***.us, ***.***.uk) <br />
com: SLD (Second-Level Domain) <br />

- admin.abd.com
admin: subdomain

- Naming rules: a-z 0-9 and hyphens (_)

### 3️⃣ Task 3: Record Types
- A record: resolve to IPv4 addresses

- AAAA record: resolve to IPv6 addresses

- CNAME record: resolve to another domain.

- MX record: resolve to the address of the servers that handle the email for the domain

- TXT record: free text fields where any text-based data can be stored.

### 4️⃣ Task 4: Making A Request
- Request a domain name => check DNS cache (return if stored) =>
request to Recursive DNS resolver (ISP) => ISP check locally (return if found) => request root DNS => TLD servers => authoritative DNS server => Resolver caches the answer => device receive & caches IP

### 🚩 Flags:
* Task 1: `Domain Name System`
* Task 2: `63`
	\- `_`
	\- `253`
	\- `ccTLD`
* Task 3: `MX`
	\- `AAAA`
* Task 4: `TTL`
	\- `recursive`
	\- `authoritative`
* Task 5: `shops.myshopify.com`
	\- `THM{7012BBA60997F35A9516C2E16D2944FF}`
	\- `30`
	\- `10.10.10.10`

<br />
<hr>
<h2 id="room-10"> 🧩🏴 Room 10: HTTP in Detail</h2>

* <a href="https://tryhackme.com/room/httpindetail">HTTP in Detail </a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: What is HTTP(S)?
- HTTPS (HyperText Transfer Protocol Secure) = HTTP + TLS encryption: data is encrypted and secure

### 2️⃣ Task 2: Requests And Responses
http://user:password@tryhackme.com:80/view-room?id=1#task3 (=URL)
- http (=scheme)
- user:password (=user)
- tryhackme (=host/domain)
- 80 (=port)
- view-room (path)
- ?id=1 (query string)
- #task3 (fragment)

### 3️⃣ Task 3: HTTP Methods
- GET Request: get info
- POST Request: create new records
- PUT Request: update info
- DELETE Request: delete info

### 4️⃣ Task 4: HTTP Status Codes
- 200: OK
- 201: Created
- 301: Found
- 400: Bad request
- 401: Not Authorised
- 403: Forbidden
- 404: Page Not Found
- 405: Method Not Allowed
- 500: Internal service error
- 503: Service unavailable

### 5️⃣ Task 5: Headers
- Request headers are additional bits of data you can send to the web server when making requests, such as, host, user-agent, content-length, accept-encoding, cookie
- Response header: returned to client from server, including set-cookie, cache-control, content-type, content-encoding.

### 6️⃣ Task 6: Cookies
Cookies: can be used to remind the web server who you are (authentication purpose)

### 🚩 Flags:
* Task 1: `HyperText Transfer Protocol`
	\- `secure`
	\- `THM{INVALID_HTTP_CERT}`
* Task 2: `HTTP/1.1`
	\- `Content-Length`
* Task 3: `POST`
	\- `PUT`
	\- `DELETE`
	\- `GET`
* Task 4: `201`
	\- `404`
	\- `503`
	\- `401`
* Task 5: `User-Agent`
	\- `Content-Type`
	\- `Host`
* Task 6: `Set-Cookie`
* Task 7: `THM{YOU'RE_IN_THE_ROOM}`
	\- `THM{YOU_FOUND_THE_BLOG}`
	\- `THM{USER_IS_DELETED}`
	\- `THM{USER_HAS_UPDATED}`
	\- `THM{HTTP_REQUEST_MASTER}`

<br />
<hr>
<h2 id="room-11"> 🧩🏴 Room 11: How Websites Work</h2>

* <a href="https://tryhackme.com/room/howwebsiteswork">How Websites Work</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: How websites work
2 components that make up a website:
- Front End (Client-Side) - the way your browser renders a website.
- Back End (Server-Side) - a server that processes your request and returns a response.

### 2️⃣ Task 2: HTML
HyperText Markup Language (HTML) is the language websites are written in

### 3️⃣ Task 3: JavaScript
Coding language allows pages to become interactive

### 4️⃣ Task 4: Sensitive Data Exposure
Sensitive Data Exposure: sensitive clear-text information can be viewed to the end-user( frontend source code)

### 5️⃣ Task 5: HTML Injection
When a website fails to sanitise user input, attackers can inject code to the inputs

### 🚩 Flags:
* Task 1: `Front End`
* Task 2: ``
	\- `HTMLHERO`
	\- `DOGHTML`
* Task 3: `JSISFUN`
* Task 4: `testpasswd`
* Task 5: `HTML_INJ3CTI0N`

<br />
<hr>
<h2 id="room-12"> 🧩🏴 Room 12: Putting it all together</h2>

* <a href="https://tryhackme.com/room/puttingitalltogether">Putting it all together </a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 1️⃣ Task 1: Putting It All Together
request a website name => Find web sever IP => connect to server => view website

### 2️⃣ Task 2: Other Components
- Load balancers: periodic checks to decide which server is best to deal with the request, also called a health check

- CDN (Content Delivery Networks): used to host static files and speed up a clients visit to a website

- WAF (Web Application Firewall): sits between the request and the web server to help against the hacking of a website. 

### 3️⃣ Task 3: How Web Servers Work
Web server: a software that listens for incoming connections and then utilises the HTTP protocol to deliver web content to its clients. Some web servers, such as, Apache, Nginx, IIS and NodeJS.

### 🚩 Flags:
* Task 1: ``
* Task 2: `CDN`
	\- `health check`
	\- `WAF`
* Task 3: `Virtual Hosts`
	\- `Virtual Hosts`
	\- `Nay`
* Task 4: `THM{YOU_GOT_THE_ORDER}`

<br />
<hr>
<h2 id="room-13"> 🧩🏴 Room 13: Linux Fundamentals Part 1</h2>

* <a href="https://tryhackme.com/room/linuxfundamentalspart1">Linux Fundamentals Part 1</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 


### 🚩 Flags:
* Task 1: ``
* Task 2: `1991`
* Task 3: ``
* Task 4: `echo TryHackMe` 
	\- `tryhackme`
* Task 5: `4`
	\- `folder4`
	\- `Hello World!`
	\- `/home/tryhackme/folder4`
* Task 6: `THM{ACCESS}`
* Task 7: `&`
	\- `echo password123 > passwords`
	\- `echo tryhackme >> passwords`

### 📌 General Notes
-
-
-

<br />
<hr>
<h2 id="room-14"> 🧩🏴 Room 14: Linux Fundamentals Part 2</h2>

* <a href="https://tryhackme.com/room/linuxfundamentalspart2">Linux Fundamentals Part 2</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 


### 🚩 Flags:
* Task 1: ``
* Task 2: ``
* Task 3: ``
	\- `down`
	\- `-h`
* Task 4: `touch newnote`
	\- `ASCII text`
	\- `mv myfile myfolder`
	\- `THM{FILESYSTEM}`
* Task 5: `user2` 
	\- `su user2`
	\- ``
	\- `THM{SU_USER2}`
* Task 6: `` 
	\- `/var/log`
	\- `/tmp`
	\- `/root` 


### 📌 General Notes
-
-
-


<br />
<hr>
<h2 id="room-15"> 🧩🏴 Room 15: Linux Fundamentals Part 3</h2>

* <a href="https://tryhackme.com/room/linuxfundamentalspart3">Linux Fundamentals Part 3</a>
* Difficulty: Easy
* Tools used: 
* Skills Learned: 

### 4️⃣ Task 4: 
- `ssh tryhackme@10.81.181.38` connect ssh
- `python3 -m http.server &` run http server, `&` run in background
- Ctrl+z and enter `bg` to run it in background
- `wget http://10.81.181.38:8000/.flag.txt` to download file
- `jobs` to view background running jobs
- `fg 1%` bring jobs back foreground 


### 🚩 Flags:
* Task 1: ``
* Task 2: ``
* Task 3: ``
	\- `THM{TEXT_EDITORS}`
* Task 4: ``
	\- ``
	\- `THM{WGET_WEBSERVER}`
* Task 5: ``
	\- `301`
	\- `SIGTERM`
	\- `THM{PROCESSES}`
	\- `systemctl enable myservice`
	\- `fg`
* Task 6: ``
	\- `@reboot`
* Task 7: ``
* Task 8: ``
	\- ``
	\- ``


### 📌 General Notes
<br /><br />
NAVIGATION 
- `whoami`: current user
- `pwd`: current path (print working directory) 
- `ls`: list files 
- `ls -a`: list hidden file (`-a`: all)
- `ls -lh`: (`-l`: list full info, `h`: human-readable)
- `cd /path/of/a/folder/`: change directory
- `cd ..` back
- `cd ~` to home directory
- `cd /root`: to root directory

<br /><br />
FILE & FOLDERS  
- `touch file.txt`: create file
- `mkdir myfolder`: make folder
- `mkdir -p fd1/fd2/fd3`: create full directory path 
	`-p` parent directories
- `cp file1.txt file2.txt`: copy file
- `cp -r folder1 folder2`: copy dir

	`-r`: recursive, itself and all its subfolders

- `mv file1.txt file2.txt`: rename file in this case
- `mv file1 file2 directory/`: move files
- `rm file.txt`: remove file
- `rm -r folder/`: remove folder safely, ask if files can't be deleted (readonly or protected) 
 
	`-r`: recursive to delete folders and all subfolders

- `rm -rf folder/`: remove folder forcely, not ask 

	`rf`: recursive forcely

<br /><br />
CONTENTS & SEARCH 
- `cat file.txt`: view file content
- `head file.txt`: view first 10 line 
- `tail file.txt`: view last 10 lines
- `find /path -name "*.log"`: file all files or dir .log in /path
- `find [/path|.] -maxdepth 1 -type f -name "*.log"`

	`.` or or `/path`: start from current dir or path. `Find` always searches recursively
	`-name`: by name
	`-type` (f|d): search file type only 
	`-maxdepth` (1|2|3|...): 1-current dir, 2-current & its child, 3 ...

- `wc -l access.log` : word count
- `grep "keyword" logfile.txt` : search string in files or directory
- `grep -r -i -n --include="*.log" "keyword" .`
- `grep -r --exclude="*.conf" "keyword" /var/log/`
<pre>
	`-i`: ignore 
	`-r`: recursive, current dir and its children
	`-l`: list file names
	`-n`: show in line number
	`-c`: number of occurrences
	`-w`: search whole word 
	`.` : start from current directory
	`--include="**.log|*.txt"` : find only
	`--exclude="*.conf|*.txt"` : exclude
	`-o "https://[^ ]*"` : print only the matching parts, `[^ ]` not space, `*` repeat n times 
	`-Eo "([0-9]{1,3}\.){3}[0-9]{1,3}"`: print IP address, `-E` Extended Regex ({}, +, |, () )
	`-v "a" file.txt`: lines not having "a", "-v" invert match. 
</pre>
- VIM & NANO

<br /><br />
PERMISSION & OPERATION
- `command 1 | command 2`: pipe, output of c1 > input of c2 

	`cat app.log | grep "error" | wc -l`

- `command 1` &: execute command 1 in the background

	ctrl + z : to stop command
	`bg` : run command in background, now can run commands simultaneously

- `command 1` && `command 2`: c2 only run if c1 succeed
- `command 1` || `command 2`: c2 only run if c1 failed
- `echo abc > myfile`: create myfile, content: abc
- `echo def >> myfile`: append myfile, content: abc def
- `./file.sh`: run file
- `file filename`: view file type
- `ssh username@MACHINE_IP`: use ssh to login to a machine
- `su username`: switch user
- `python3 -m http.server`: run http server
- `wget http://10.81.181.38:8000/.flag.txt`: download file
- `scp important.txt ubuntu@10.81.181.38:/home/ubuntu/transferred.txt` upload from local
- `scp ubuntu@10.81.181.38:/home/ubuntu/documents.txt notes.txt` copy from remote
-
<br />
<hr>
<h2 id="room-0"> 🧩🏴 Room 0: </h2>

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
* Task 1: ``
	\- ``
	\- ``
* Task 2: ``
	\- ``
	\- ``
* Task 3: ``
	\- ``
	\- ``
* Task 4: ``
	\- ``
	\- ``


### 📌 General Notes
-
-
-


---







