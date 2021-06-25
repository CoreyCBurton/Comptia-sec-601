# Exploring the Lab Environment
- There are different VMs that vary from servers to different operating systems.
  - The screenshot below shows what VMs are available.
  ![Capture](https://user-images.githubusercontent.com/81980702/121715541-9f3db200-caa4-11eb-9be9-dd06c3a497d7.JPG)


# Help center
- The screenshot below shows what the help center offers for any issues.
   ![image](https://user-images.githubusercontent.com/81980702/121715697-cbf1c980-caa4-11eb-8de4-0abd80d91ab7.png)

# Change resolution
- In the top left, the icon with the computer can change what VM is selected.
![image](https://user-images.githubusercontent.com/81980702/121715908-08bdc080-caa5-11eb-96aa-410d2b2a3776.png)

# Lightning icon 
- The lightning icon allows you to have windows keys. For example, alt+control+delete can be accessed ![image](https://user-images.githubusercontent.com/81980702/121716174-55a19700-caa5-11eb-8be8-49f4f7cec858.png)

# DC1
- DC1 is the main domain controller (DC)
  - This is unusual, it should not be combined with other roles but this lab is used for convenience
  - The static IP address is (10.1.0.1)

# MS1
- MS1 is a mail server for running applications. It runs a DHCP service to perform auto addressing for clients
  - It has the webserver Internet Information Services (IIS) and the email server hMail.
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
- the path to see if IPv4 mode is Tools > DHCP.

![image](https://user-images.githubusercontent.com/81980702/121719293-7a4b3e00-caa8-11eb-99df-3065caeb42f2.png)
> The IPv4 has a green tick which shows that it is active 

# Load a DVD drive
- Clicking in the icon below loads a CD onto the VM. 
![image](https://user-images.githubusercontent.com/81980702/121720430-ba122580-caa8-11eb-8702-96099ea15f00.png)

# Powershell commands
- The commands below are executed in Powershell
  - ``hostname`` returns ``MS1``
  - ``Get-NetIPAddress`` returns the IPv4 address which is ``10.1.0.2``

# Using Kali Linux (PT1-Kali)
- Log in with root

# Web server and open local website (Kali)
- using command ``systemctl start apache2`` and ``firefox http://localhost``
  - The local host is shown below
![image](https://user-images.githubusercontent.com/81980702/121721281-b4690f80-caa9-11eb-8efa-a87e92347c69.png)

# Different appliance VMs
- RT1-LOCAL | RT2-ISP | RT3-INT 
  - Running VyOS Linux distribution to route traffic between different subnets

- UTM1
  - Security appliance created by Netgate 
  - GUI is used on http://10.1.0.254

- SIEM1 
  - Security onion monitoring tool

- LAMP is built on the Ubuntu Server 

- LX1
  - CentOS linux distrubution with vulnerable web services 

# Powershell on MS1
- command ``ipconfig /all >$env:USERPROFILE\Desktop\ipconfig.txt`` outputs this file below 

![image](https://user-images.githubusercontent.com/81980702/121722340-f181d180-caaa-11eb-9179-b3ee008e1073.png)

# Primary DNS Suffix
![image](https://user-images.githubusercontent.com/81980702/121722475-1bd38f00-caab-11eb-98ce-cb49a59914b4.png)


