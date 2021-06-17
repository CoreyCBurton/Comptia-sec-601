# Sign into Kali Linux
- Use root to sign in

# ifconfig
- eth0 is shown below 
- ![image](https://user-images.githubusercontent.com/81980702/121723552-4540ea80-caac-11eb-888e-c5d4198cd0bb.png)

- ``ip a`` also shows this information
  - This is the new version of ifconfig 
  - The ip address is ``10.1.0.192``

# ip route show
- ![image](https://user-images.githubusercontent.com/81980702/121723753-889b5900-caac-11eb-8e4e-9736bc0a2d70.png)
- The IP for the router is 10.1.0.254
  - The connection uses DHCP to provide the client addresses 

# arp -a
- The address Resolution Protocol on this vm is 10.1.0.1
  - Checks the ARP cache to display other hosts local to the subnet
- ![image](https://user-images.githubusercontent.com/81980702/121723909-bda7ab80-caac-11eb-8d56-519cbe325239.png)

# ip neignbor
- command ``ip neighbor`` preforms a sweep of the local network. 
  - you can also use ``netdiscover`` in kali linux

# netdiscover 
- Using command ``netdiscover -i eth0 -r 10.1.0.0/24``
  - This list 5 different IP addresses 

# ipconfig (Windows)
- command ``ipconfig`` returns ip addresses
  - The IPv4 for DC1 is ``10.1.0.1``

# Pathping
- `` Command pathping 10.1.0.192`` returns the screenshot below 
- ![image](https://user-images.githubusercontent.com/81980702/121973589-40499880-cd43-11eb-893a-bf520e066a14.png)
- **Please note** - 0 packets have dropped

# NMAP
- Using kali linux and the command `` nmap localhost`` it shows open ports
  - Port 22 is open 

- ``nmap 10.1.0.0/24`` shows a list of ports that are open on the network

- Using command ``nmap -A 10.1.0.254`` shows this in the screen shot below 
- ![image](https://user-images.githubusercontent.com/81980702/121973951-fca35e80-cd43-11eb-83f5-97cdcf30bf5e.png)

- command ``nmap -p 20-200 10.1.0.0/24`` scans the 20-200 ports
- ![image](https://user-images.githubusercontent.com/81980702/122444912-a2ceae80-cf66-11eb-8c67-4e3f22755d56.png)
- Port 80 is open on 10.1.0.0

- ``nmap --top-ports 20 10.1.0.0/24``scans the most common ports
- ![image](https://user-images.githubusercontent.com/81980702/122445304-0bb62680-cf67-11eb-8464-bd7931f6584a.png)

- ``nmap -sn 10.1.0.0/24`` scan up and down ports 
- ![image](https://user-images.githubusercontent.com/81980702/122445653-5e8fde00-cf67-11eb-8fbd-9411dc2f4510.png)

# cURL command 
- Banner grabbing is a way of identifying service versions. This information helps attackers select potentially vulnerable machines.
  - ``curl -s -I 10.1.0.1``
- ![image](https://user-images.githubusercontent.com/81980702/122446063-dbbb5300-cf67-11eb-9435-6fb57dd990fd.png)
- It is running IIS 10

# Firefox
- Using command ``firefox http://10.1.0.1`` you can see what the server is running on a browser.
- ![image](http://10.1.0.1s.githubusercontent.com/81980702/122446466-4f5d6000-cf68-11eb-9104-5fdc54bd3cc3.png)

# Dig
- These name records can also reveal information about how a network is configured. In this task, you will gather DNS information by using the dig utility.

- command ``dig -x 10.1.0.254``
- ![image](https://user-images.githubusercontent.com/81980702/122446868-c1ce4000-cf68-11eb-9023-5313bc754373.png)
- 10.1.0.1 is the server that answers the query 

















