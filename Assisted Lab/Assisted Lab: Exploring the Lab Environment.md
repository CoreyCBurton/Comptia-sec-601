# Exploring the Lab Environment
- Used to show VMs 
  - Loaded on a ISO disc inage 
  
![Capture](https://user-images.githubusercontent.com/81980702/121715541-9f3db200-caa4-11eb-9be9-dd06c3a497d7.JPG)
> The navation center

# Help center
- what the help center looks like
  - ![image](https://user-images.githubusercontent.com/81980702/121715697-cbf1c980-caa4-11eb-8de4-0abd80d91ab7.png)

# Change resolution
- In the top left, this icon changed the screen size and reconnect
![image](https://user-images.githubusercontent.com/81980702/121715908-08bdc080-caa5-11eb-96aa-410d2b2a3776.png)

# Lightning icon 
- The lighning icon allows you to have windows keys can commands ![image](https://user-images.githubusercontent.com/81980702/121716174-55a19700-caa5-11eb-8be8-49f4f7cec858.png)

# DC1
- DC1 is the domain controller (DC)
  - This is unusual, it should not be combined with other roles but this lab is used for convience 
  - THe static ip address is (10.1.0.1)

# MS1
- A member server for running applications. It runs a DHCP service to perform auto addressing for clients
  - It has the web server Internet Information Services (IIS) and the email server hMail
  - The static IP address is 10.1.0.2

# Username and Password
- Username
  - 515support\Administrator

- Password
  - Pa$$w0rd 

# Network connection (DC1)
![image](https://user-images.githubusercontent.com/81980702/121717988-69e69380-caa7-11eb-9eea-a27bc901a4df.png)
> The network connection recognizes it as corp.515support.com

# IPv4 node
- Tools > DHCP.

![image](https://user-images.githubusercontent.com/81980702/121719293-7a4b3e00-caa8-11eb-99df-3065caeb42f2.png)
> The IPv4 has a green tick 

# Load a DVD drive
- Clicking in the icon below loads a cd.
![image](https://user-images.githubusercontent.com/81980702/121720430-ba122580-caa8-11eb-8702-96099ea15f00.png)

# Powershell commands
- ``hostname`` returns ``MS1``

- ``Get-NetIPAddress`` returns the IPv4 address which is ``10.1.0.2``

# Using Kali Linux (PT1-Kali)
- Log in will be root and Pa$$w0rd

# Web server and open local website (Kali)
- using command ``systemctl start apache2`` and ``firefox http://localhost``

- The local host is shown below
![image](https://user-images.githubusercontent.com/81980702/121721281-b4690f80-caa9-11eb-8efa-a87e92347c69.png)

# Different applaince vms
- RT1-LOCAL | RT2-ISP | RT3-INT 
  - Running VyOS linux distribution to route traffic between different subnets

- UTM1
  - Security appliance created by Netgate 
  - GUI is used on http://10.1.0.254

-SIEM1 
 - Security onion monitoring tool

- LAMP is built on the Ubuntu Server 

- LX1
  - CentOS linux distrubution with vulnerable web services 

#Powershell on MS1
- command ``ipconfig /all >$env:USERPROFILE\Desktop\ipconfig.txt`` outputs this file below 

![image](https://user-images.githubusercontent.com/81980702/121722340-f181d180-caaa-11eb-9179-b3ee008e1073.png)

# Primary DNS Suffix
![image](https://user-images.githubusercontent.com/81980702/121722475-1bd38f00-caab-11eb-98ce-cb49a59914b4.png)

