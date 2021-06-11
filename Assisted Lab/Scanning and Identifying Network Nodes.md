# Sign into Kali Linux
- Use root to sign in

# ifconfig
- eth0 is shown below 
![image](https://user-images.githubusercontent.com/81980702/121723552-4540ea80-caac-11eb-888e-c5d4198cd0bb.png)

- ``ip a`` also shows this information/
  - This is the new version of ifconfig 
  - The ip address is ``10.1.0.192``

# ip route show
![image](https://user-images.githubusercontent.com/81980702/121723753-889b5900-caac-11eb-8e4e-9736bc0a2d70.png)
- The IP for the router is 10.1.0.254
  - The connection uses DHCP to provide the client addresses 

# arp -a
- The address Resolution Protocol on this vm is 10.1.0.1
  - Checks the ARP cache to display other hosts local to the subnet
![image](https://user-images.githubusercontent.com/81980702/121723909-bda7ab80-caac-11eb-8d56-519cbe325239.png)

# ip neignbor
- command ``ip neighbor`` preforms a sweep of the local network. 
  - you can also use ``netdiscover`` in kali linux

# netdiscover 
- Using command ``netdiscover`` -i eth0 -r 10.1.0.0/24
