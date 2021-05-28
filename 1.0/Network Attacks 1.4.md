# Rogue access point
* An unauthorized wireless access point 

* May be added by an employee or an attacker 

* A significant backdoor

* A very easy to plug in a wireless AP

> Schedule a periodic survey and consider using 802.1X(Network Access Control)

# Evil twins
* Looks legitimate but malicious

* Configure an access point to look like an existing network

* Overpower the exisitng access points 

* WiFi hotspots are easy to fool

# Bluejacking 
* Sending of unsolicited messages to another device via bluetooth 

* Typical functional distance is about 10 meters 

* Bluejack with an address book object

> Low security but attackers can still send messages 

# Bluesnarfing 
* Access a Bluetooth-enabled device and transfer data

* First major security weakness in Bluetooth

> Older device has access to bluetooth cam be vulnerable

# Wireless Disassociation 
* The network keeps on disappearing; you are not able to stop it

* Wireless deauthentication; denial of service attack

> 802.11 management frames allow you to find access points and manage Qos. 

# Wireless jamming
* Many different types; contant, random bits / constant, legitimate frams

* Sent at random times and Reactive jamming; When someine tries to communicate

* Needs to be somewhere close 

# Radio frequency (RF) jamming 
* Denial of service 

* Transmit interfering wireless signals
> Decreases the signal-to-noises ratio at the receiving deive

* Sometimes its not intentional but can be intentinoal 

# Radio-frequency identification(RFID)
* They are everywhere; They are used anywhere to track

* Radar Technology; No battery 

> RFID attacks can involve data capture, spoof the reader, denial of service, and decrypt communication

# Near field communication (NFC)
* Two-way wireless communication 

* payment systems 

* Bootstrap for other wireless; a token 

> Remote capture, Frequency jamming, Relay; on path attack 

# Initialization vector
* An input to a cryptographic primitive being used to provide the initial state. 

* Attack on wireless network that modifies the IV of a encrpyed packet. The attacker can learn the plaintext of one packet then compute the RC4 key. 

# MAC address
* The physical address of a network adapter 

* 48 Bits / 6 bytes long

* Example: 8c:2d:aa:4b:98:a7 8C:2d:aa = Manufactur model number 4b:98:a7 = Serial number (speicifc to the address)

> Lan switching 
* foward or drop frames; Based on the MAC address 

* Gather a list of MAC addresses 

* Maintains a loop-free environment ( Using spanning tree protocol ) 

* The sources mac address and destinational mac address get sent to the switch 

* The switch makes a table of MAC addreses which directs traffic 

# MAC flooding 
* The mac table is only so big 

* Attackers send info to the mac table and fill it up which turns the switch into a hub. The hub then can capture all network for a hacker to take advantage.

# MAC cloning
* attacker modifies the mac address to match the mac address of the legitimate device

* Create a DoS; Disrupt coomunication to the legit MAC

* Manipulate through software 

# Address resolution protocol (ARP) poisoning
* Links addressed to the right places

* when you ping another computer through the terminal, it sends arp request 

* on path attack that can receives data from two different computers

# DNS poisoning (spoofing)
* Modifys the information in a DNS server

* Modifty the client host file 

* Send a fake response to a valid DNS request 

> The bad guy changes the DNS server actively

# Domain hijacking
* Gets access to the domain registration and you have control of where the traffic flows 

* Brute force is used, Social engineering the password, gains access to the email address

> The domain change in a brazilian bank left the hacker under control for 6 hours. The bank had 5 million customers and 27 billion in assets. 

# Universal resource locator (URL) redirection
* Unique identifier used to locate a resource on the internet. It is also referred as a web address

* Hacker redirects the URL to a malicious website

# Domain reputation
* A concept where in a domain repuatation API, or a similar program is able to assess the reputation of a domain or IP address using a set of data resources.

* It is used to accept and reject connections.

# Distributed denial-of-service (DDoS)
* Force a server to stop working 

* Takes a design failure or vulnerability 

* can be caused for a creative advantage 

* can be used to create a spoofing attack 

* can be created by accident; loop or even downloading a big file

* can be caused with botnets 

> Application DoS
* Makes the application break or work harder 

* a zip bomb can be used in an Application Dos and even cloud base services

> Operational Technology (OT) DoS
* the hardware and software for industrial equipment 

* Powergrid can stop operate and even traffic lights can turn all green which is hazardous 

# Malicious scripts 
* Automate task and they have alot of speed 

> Powershell
* .ps1 file extension 

* Extends command line function 

* Attacks windows OS

> Python
* General-purpose scripting language 

* Popular in alot of tech and used for cloud orchestration

* Attacks infrastructure; Routers, switches, and servers

> Shell script 
* Automate and extend the command line 

* Starts with a shebang

* Attack Linux/unix environments

* Controls the os on the command line 

> Macros 
* Automate functions inside an application 

* Attackers create exploits that execute with macros 

> Visual Basic For Applications
* Automates processes in a Windows application 

* Code can be run through these processes; very vulnerable. 