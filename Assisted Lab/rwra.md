# Intro
- In this activity, you will use Wireshark and tcpdump to capture network traffic and display relevant information on the local network. Interpreting the output from such captures is useful for security assessments.

# Kali linux
- Log in to kali linux
  - Select the Wireshark for the application
  - ![image](https://user-images.githubusercontent.com/81980702/122490323-5d7ea100-cfa7-11eb-82b2-e9d2ffa01036.png)

- Under capture Select Eth0 adapter
  - Under the filter box type IP
  - This shows IPv4 traffic, not IPv6

# Opening Firefox
- Using command ``firefox http://10.1.0.2`` this opens up the server
  - There will be packets captured when opening up wireshark
![image](https://user-images.githubusercontent.com/81980702/122490641-15ac4980-cfa8-11eb-80e2-2693bbc00834.png)

# What wireshark captures 
- Framet
  - this shows information about the bytes captured.

- Ethernet II
  — this shows the frame type (data link layer/layer 2) and the source and destination MAC addresses. Note that the first part of the address (the OUI) is identified as belonging to Microsoft (all the VMs are using MS virtual adapters). The last piece of information is the type of network protocol contained in the frame (IPv4).

- Internet Protocol Version 4
  — this is the IPv4 datagram, notably showing the source and destination IP (layer 3) addresses. Note there is usually also a GeoIP function in this section, but as these are private addresses, they cannot be resolved to a particular regional registry or ISP.

- User Datagram Protocol
  — layer 4 (transport) uses either UDP or TCP. The most significant fields here are the source and destination ports. UDP port 53 is the "well known" DNS server port.

- Domain Name System
  — this is the application protocol. Depending on which frame you selected, you may be looking at a query or at a response.
  
![image](https://user-images.githubusercontent.com/81980702/122508878-5320cf00-cfc8-11eb-9cb9-734b2997d15d.png)

# The TCP frame connecting to 10.1.0.2
![image](https://user-images.githubusercontent.com/81980702/122508979-8cf1d580-cfc8-11eb-83ab-00fd46d5908a.png)

- Ethernet II is where the mac addresses are found

- Internet Protocol Version 4 is where the IP addresses are found

- Transmission Control Protocol (TCP) is where destination port numbers are found.

# MS1 Server Manager
- Tools > Internet Information Services (IIS) manager
  - Go into the sites node 
![image](https://user-images.githubusercontent.com/81980702/122509580-a5aebb00-cfc9-11eb-8f5c-5b1e54d8733c.png)

- Disable Anonymous Authentication and Enable Basic Authentications
  - SSL is not enabled for this site so credentials will be sent in clear text 

![image](https://user-images.githubusercontent.com/81980702/122509742-e3abdf00-cfc9-11eb-8f42-454c51e9cdd1.png)










