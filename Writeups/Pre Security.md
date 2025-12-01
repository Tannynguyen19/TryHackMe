###### <h2>🏴 Pre Security</h2> 

> Writeups for TryHackMe <br />
> Author: Tanny Thanh Nguyen

<br />
<h2>📚 Table of Contents</h2>

\- [Room 1: Offensive Security Intro](#room-1-Offensive-Security-Intro)

\- [Room 2: Defensive Security Intro](#room-2-Defensive-Security-Intro)

\- [Room 3: Careers in Cyber](#room-3-Careers-in-Cyber)

\- [Room 4: What is Networking?](#room-4-What-is-Networking?)

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
* Task 2:
* Task 3:
* Task 4:


### 📌 General Notes
-
-
-


---







