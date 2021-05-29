# Ransomeware
- A type of malware that threatens to publish the victim's data or block access unless the ransom is paid. 
  - **Crypto malware** is used to block access 
 
- To counter ransomware, make sure you backup of your information. It does take time for you to reset which can cost the company money.

  - **Example** - Cerber is a RaaS platform that appeared in 2016. Cerber took advantage of a Microsoft vulnerability to infect networks. It used AES-256 algorithm to infect backups and personal data. Darkside is also another Ransomeware that has appeared in 2020. 
 

# Trojans 
- The origin of the name Trojan comes from the Greeks and how they captured Troy by hiding in a big wooden horse.

- The software looks completely normal, the goal is to trick the user into running the software such as a spreadsheet or a game but it actually is a virus hence the name Trojan. 
  - The virus is usually hidden from your antivirus and shuts it off in some situations.

- The virus can install a **backdoor** which allows the attacker to gain access into the system again. 

# Remote Acess Trojans (RAT) 
- With a Trojan being installed, a remote administration tool is given to the attacker. 
  - Keylogging, screen recording, copy files, embed more malware can be done through this remote administration tool.

- **Example** - Darknet, a remote access trojan (RAT) developed by Jean-Pierre Lesuer that allowed a user to control a system with a graphical user interface. Tracks users by taking screen captures, keylogging, or password stealing. 

![image](https://user-images.githubusercontent.com/81980702/120059197-87325100-c015-11eb-936f-224875427f3c.png)
> Image of SubSeVen, A RAT interface, 

# Potentially unwanted programs (PUPs) 
- PUPs are unwanted programs installed from another installer in most cases
  - Most anti-virus can identify PUPs
  
- **Examples** - Software backups, toolbar applications, and many more unwanted programs.

# Worms
* Malware that self-replicates

* Uses a network as a transmission medium

* The worm takes over systems very quizkly 

* Firewalls can stop many worm infestations

> The Wannacry worm happened in 2017, it installed crypto malware on computers which were then held for ransom. The worm was able to spread to multiple computers. To spread, there was no human intervention involved 

# Fileless virus
* It is a stealth attack

* Operates in memoery

> user clicks on a malicious website link. Website exploits a Flash/Java/Windows vulnerability. 	Launches PowerShell and downloads payload. Runs PowerShell scripts and executes in memory. Adds an auto start to registry.

# Command and Control
* A computer controlled by an attacker which is used to send commands to systems compromised by malware and receive stolen data from a target network

* Cybercriminals use them as a headquarters for compromised machines in a botnet

> A computer gets compromised and becomes the control center. That computer then starts recruiting bots.

# Bots 
*	When your system is infected, it becomes a bot.

*	Bots are usually installed by a trojan horse. 

*	The bots work together and waits for commands from the command-and-control center 

*	The groups work together in a bot net and can cause DDoS attacks, relay spam, and other type of computing task 

*	Botnets are for sale

> The website https://map.lookingglasscyber.com/ shows what botnets are active and possible attacks. 

# Logic Bomb 
•	Waits for a predefined even

•	Often left by someone with a grudge with a company 

•	The logic bomb can follow time or date or is a user event

•	Logic bombs are hard to trace, there is no digital signature 

> In 2013 in South Korea, an email sent to employees had a trojan horse virus attached to it. A day later, the logic bomb went off. Storage and master boot records were deleted off devices showing error “Please install operating system”

# Spyware  
•	Malware that spies on you, advertising, identity theft, affiliate fraud

•	Often is a trojan horse 

•	Some spyware has keyloggers 

> info stealers is a type of malware to scan infected computers and steal personal information. 

# Roolkit  
•	Originally a Unix technique 

•	Modifies core system files in the kernel of a system

•	Become invisible to traditional malware detection

> Zues/zbot malware was famous for cleaning out bank accounts. The Zbot combines with Necurs Rootkit which makes it impossible to delete zbot. 

# Spraying Attack 
•	Try to log in with an incorrect password till they get locked out

•	The attacker uses common passwords 

•	If the common passwords do not work, they will move on to the next account after it is locked 

# Dictionary  
•	Uses a dictionary to find common words 

•	Common passwords that are made by humans

•	There are dictionaries online that are common passwords for someone who works at a specific company. The attacker will then use that to target someone from the company they are looking at. 

•	The dictionary password attacks can substitute letters such as “p&ssw0rd” 

•	Takes time 

> Discovers common passwords and their hash attached to it such as ninja, dragon, football, letmein. 

# Brute force 
•	Tries every password combination until the hash is matched 

•	A strong hashing algorithm slows things down 

> The attacker obtains a file and the hashes with the passwords. They will then use brute force against the hash with multiple letter combinations 

> **Online** 
•	Very slow 

•	Most accounts will be locked out	

> **Offline** 
•	Obtains a list of users and hashes 

•	Calculates a password hash and compares it to a stored hash

•	Requires a lot of resources 

# Rainbow tables 
•	An optimized, prebuilt set of hashes. 

•	Doesn’t contain every hash

•	Contains pre-calculated hashes 

•	Speeds processes 

•	You will have to have different rainbow tables for different hashing methods. Windows is different from MySQL.

# Malicious universal serial bus (USB) cable 
•	Looks like a normal USB cable 

•	Operating system identifies it as a HID or a human interface Device, A keyboard doesn’t need extra rights or permissions. 

•	Plug in usb cables that only you trust. 

# Malicious flash drive
•	A free usb flash drive can a virus on it. It is a bad idea to plug on a flash drive when you do not know what is on it

•	Older operating system would automatically run files 

•	Additional electronics inside an infected flash drive can make the computer automatically run a program. 

> Attackers can load malware in documents. Can be configured as a boot device. Acts as an ethernet adapter

# Skimming 
•	Stealing credit card information, usually during a normal transaction 

•	Copies data from a magnetic strip, card number, expiration date, and card holder’s name

> ATM skimming that includes a small camera to watch for pins or puts a fake card reader that looks like it is a part of the device when it is actually there just to steal information.

# Card cloning 
•	Usually gets the credit card details from a skimmer 

•	Creates a duplicate of a card that only has a strip, the chip cannot be replicated. 

•	Gift cards are common with card cloning. 

# Adversarial artificial intelligence (AI)
•	Requires a lot of data training 

•	Recognizes pattern with the data that is collected 

•	Used to stop spam, recommend products to an online retailer, prevent car accidents. 

# Supply chain attacks 
•	The supply chain consist of raw materials, manufactures, distributions, and customers

•	Attackers can infect any step along the way. People trust their suppliers 

•	One exploit can affect the whole supply chain 

> 40 million credit card numbers where stolen from a supply chain. It started with a HVAC ac company. The attackers then got into Targets network

# Cloud-based vs. on-premises attacks
•	Attacks can happen in two places, on premises or on the cloud

•	Cloud base security, everything is centralized with no cost 

•	On premise security puts a burden on the client with data center security and infrastructure cost.

•	On base security allows people in the company to change security while the cloud is upheld with a third party. 

# Cryptographic attacks
•	Data is encrypted 

•	The bad guy doesn’t have the key to the encrypted data 

•	Attackers spend a lot of time trying to decrypt 

# Birthday attack 
•	There 23 students in a classroom. What are the chances of them having the same birthday? It is %50. For 30 it is %70. 

•	A hash Collison is when you have two different plaintext but they have the same hash. 

•	When the hash collusion is found, brute force can be used 

# Collisions 
•	Hashes are supposed to be unique; different input data shouldn’t create the same hash 

•	Message Digest Algorithm 5 had collisions

# Downgrade attack
•	Instead of using good encryption, you use something that is not great

•	In 2014 a TLS vulnerability POODLE, they forced the encryption to SSL3.0 which has vulnerabilities. 
