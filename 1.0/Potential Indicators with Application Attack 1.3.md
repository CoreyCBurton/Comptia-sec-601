# Privilege escalation
* Gains full access to a system

* exploits a vulnerability 

* Ussally when one user can access another user 

* Malware can catch any privilage escalation 

> CVE-2020-1530 Windows Remote Access Elevation of Privelage vulnerability august 20, 2020

# Cross-site scripting
* Also known as **XSS** 

* Orginally associated with a browser security flaws; Information from one site to another could be shared

* Common web based application developement errors

* Malware used in javascript

* Non-persistant XSS attack 

> seach box is a common source 
> Sent through link that activates payload 
> Hacker can get session id and more information

* Persistent XSS attack 

> Includes a malicious payload 
> The malicious message has the virus and everyone gets it when the message is read 
> There isnt someone targeted; different from non-persistant where the person can be targeted 
> Can spread easy through social media

> Example- Subaru website gave you a log in token when you entered the website. The log in token never expired, therefore if someone got ahold of this token, theu could log in. 

# Injection
* Adding your own information in a data stream 

* Enabled because of bad programming 

* Different data types such as HTML,SQL,XML,LDAP,etc.

# SQL injectionv
* Also known as Structured Query Language

* Relational database management language

* Modifiying SQL request 

* Application shouldnt allow this 

> A log in with username and password with a website. Authentication token doesn’t verify so you can add or "1"=1 which will pull up all the data. 

# DLL injection 
* Also known as Dynamic-Link Library 

* A windows library containing code and data 

* Inject a DLL to have an application run a program 

> The hacker will inject data into a process that will then create a new thread which will give the hacker more rights then he has.

# XML injection 
* Extensible Markup Language 

* transfer data between two different devices

* Modify XML request, a good system can valiadte if the request is valid

# LDAP injection
* Also known as Lightweight Directory access protocol 

* Used to store data like username and password 

* You can gather information by modifiying request

# Pointer/object dereference
* An object in programming thats stores memory in another address or another value located in computer memory

* When it retrieves value, it is known as dereference. 

* The hacker tries to get value located in a computer memory

#  Directory traversal attack
* an HTTP attack which allows attackers to access restricted directories. 

* Two levels of security; Access control list and Root Directory 

* The hacker takes advatange of this 

# Buffer overflows
* When one section of memory overwites another bit of memory

* Takes advantage of poor programming; devs need to preform bound checking 

* Takes time to avoid crashing 

* A hacker can take advantage of an empty string thar overflows in another value. This can give the hacker access that he wouldnt have had previously before

# Race conditions
* Happens when a computing system that is designed to handle task is forced to preform two or more operations. 

* The technique takes advantage of a time gap that allows the security to lag behind. **Time of check/time of use**.

> in the 1980s, a race condition in a threapy machine caused 100 times the normal dose of radiation. 

# Error handling
* Improper handling of errors can lead to security problems

* Detailed error message include on potential flaws, stack traces, database dumps, and error codes. Can point a hacker in the right direction

# Improper input handling
* Poor input can cause alot of security vulnerabilities 

* proper validation is to identify the correct form of data

* Devs need to check to make sure that every input doesn’t allow SQL injections, buffer overflows, denial of service, etc. 

* Takes alot of work to find the input. 

# Replay attack
* Useful information is transmitted over the network 

* The attacker needs access to raw network data; Network tap, ARP poisoning, Malware on the victums computer

* They gather informatiom to help the attacker; they replay the data to appear as someone else 

* Not an on-path attack; doesnt require the orginal workstation. 

> Pass the hash: The client sends a hash to the server which is then caught by the attacker. The attacker then sends the hash back. 

# Session replays
* The hacker gets access to the session Id; The user has the session so he can avoid log ins every time they enter the site. 

* The hacker uses this session ID to then log into the web server. 

# Integer overflow
* When a value is moved into variable that is too small to hold it. 

* Downcasting from a long to an int is an example. 

# Cross-site requests 
* Cross-site request are common and legitimate; a browser can load stuff from youtube, instagram, and other text

* HTML on a website can direct request from your browser which is fine 

* Alot of request are unauthenticated

> Client side: Renders the page on the screen; HTML, JavaScript
> Server side: Performs requests from the client: HTML,PHP; Transfer money from one account to another

# Cross-site request forgery
* One-click attack, session riding; XSRF,CSRF

* Takes advantage of the trust that a web application has for the user; The website trust your browser, The request are made without consent; Attacker can post a facebook status

* Web application needs to have anti-forgery techniques. 

> Server side request: Attacker finds a vulnerable web application; sends request to a web server; Web server performs the request on behalf of the attacker

# Application programming interface (API) attacks
* Attackers look for vulnerabilites in this communication path

* sensitive data, DoS, intercept communication, privileged access

* API request from a phone instead of a HTTP computer

# Resource exhaustion
* A specialized DoS attack 

> ZIP bomb; 42 kilobyte .zip compressed file. When uncompressed, it is 4.5 petabytes; identify by antivirus. 
> DHCP Starvation; Attacker floods network with IP address requests. MAC address changes so the DHCP server will eventually run out of addresses 

# Memory leak 
* Unused memory is not properly is not released

* Begins to grow slowly in size 

* Systen crashes 

# Secure sockets layer (SSL) stripping
* Combines on-path attack with a downgrade attack

* Attacker sits in the middle of the attack with the client and server

* Proxy server, ARP spoofing, Rouge WI-FI hotspot

* Software and browser needs to be updated to be countered

> To counteract this, the user and the server expect to receive an HTTPS instead of HTTP which stops the man in the middle attack.

# Driver manipulation
* Drivers are powerful, they are often trusted. 

> Shimming: A fit in the gap. A middle man
* Windows has a shim which allows older application to run in the new version of windows

* Malware takes advantage of shims 

> Refactoring 
* A different program each time it is downloaded

* Make it appear different everytime; Add useless code

* All this is used to mask against an antivirus software