# Intro
- In this lab, The user will use Wireshark and tcpdump to capture network traffic and display relevant information on the local network. 
	- Interpreting the output from such captures is useful for security assessments.

# Kali Linux
- Log in to Kali Linux
  - Select the Wireshark for the application

![image](https://user-images.githubusercontent.com/81980702/122490323-5d7ea100-cfa7-11eb-82b2-e9d2ffa01036.png)

- Select the Eth0 adapter
  - This shows IPv4 traffic, not IPv6

# Opening Firefox
- Using command ``firefox http://10.1.0.2`` 
	- This opens up the server
  - There will be packets captured when opening up wireshark
![image](https://user-images.githubusercontent.com/81980702/122490641-15ac4980-cfa8-11eb-80e2-2693bbc00834.png)

# What Wireshark captures 
- Framet
  - this shows information about the bytes captured.

- Ethernet II
  - this shows the frame type (data link layer/layer 2) and the source and destination MAC addresses. Note that the first part of the address (the OUI) is identified as belonging to Microsoft (all the VMs are using MS virtual adapters). The last piece of information is the type of network protocol contained in the frame (IPv4).

- Internet Protocol Version 4
  - this is the IPv4 datagram, notably showing the source and destination IP (layer 3) addresses. Note there is usually also a GeoIP function in this section, but as these are private addresses, they cannot be resolved to a particular regional registry or ISP.

- User Datagram Protocol
  - layer 4 (transport) uses either UDP or TCP. The most significant fields here are the source and destination ports. UDP port 53 is the "well known" DNS server port.

- Domain Name System
  - this is the application protocol. Depending on which frame you selected, you may be looking at a query or at a response.
  
![image](https://user-images.githubusercontent.com/81980702/122508878-5320cf00-cfc8-11eb-9cb9-734b2997d15d.png)

# The TCP frame connecting to 10.1.0.2
![image](https://user-images.githubusercontent.com/81980702/122508979-8cf1d580-cfc8-11eb-83ab-00fd46d5908a.png)

- Ethernet II is where the mac addresses are found

- Internet Protocol Version 4 is where the IP addresses are found

- Transmission Control Protocol (TCP) is where destination port numbers are found.

# MS1 Server Manager
- The path to follow is Tools > Internet Information Services (IIS) manager
  - Go into the sites node 
![image](https://user-images.githubusercontent.com/81980702/122509580-a5aebb00-cfc9-11eb-8f5c-5b1e54d8733c.png)

- Disable Anonymous Authentication and Enable Basic Authentications
  - SSL is not enabled for this site so credentials will be sent in clear text 

![image](https://user-images.githubusercontent.com/81980702/122509742-e3abdf00-cfc9-11eb-8f42-454c51e9cdd1.png)

# TCPdump
- This is being ran in Kali Linux
  - Command `` tcpdump -vv dst 10.1.0.2 and port www -w ww.pcap`` listens for packets
  - The packets will be directed to the file www.pcap

- For this example, I visted the 515 support server
  - ctrl+C to stop the tcp dump 
  ![image](https://user-images.githubusercontent.com/81980702/122579302-63fa3080-d01a-11eb-9d3e-fd6937b6a3ce.png)

- Opening the PCAP file that was collected in wireshark brings this 
![image](https://user-images.githubusercontent.com/81980702/122579486-9310a200-d01a-11eb-92d6-c67a54290b2a.png)

- You can find the credentials we used through this method 

# Tcpdump SSH 
- command `` tcpdump -vv dst 10.1.0.10 and port ssh -w ssh.pcap `` captures ssh packets

- Through a second window, I am going to connect to root by `` ssh root@10.1.0.10`` and use the default password
![image](https://user-images.githubusercontent.com/81980702/122580495-a2441f80-d01b-11eb-915e-b42fe23abb9e.png)

- The packets captured is listed below 
![image](https://user-images.githubusercontent.com/81980702/122580729-e3d4ca80-d01b-11eb-90de-edfe26ebdcf1.png)

# Conclusion
-  Viewed HTTP and SSH traffic

- HTTPS stops outside listeners from getting this information. 












