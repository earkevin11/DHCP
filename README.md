# DHCP

# What is DHCP?
- DHCP stands for Dynamic Host Configuration Protocol
- DHCP is a network management protocol that allows <em> servers <em> used to dynamically assign an Internet Protocol (IP) address to any device, or node, on a network so they can communicate using IP.
- In Windows, one must install DHCP server role on a Windows Server Server to have the functionality on the network.
- Allows automatic TCP/IP configuration
  
 # Example of DHCP
  - Getting a room in a hotel
  - DHCP lease - IP addresses are not permanent but are rented out. Like a room in a hotel.
  - DHCP Clerk knows which rooms (IP addresses) are available and what is reserved.
  - When a client's computers DHCP expires, it comes back to the server for and either extends existing IP address or DHCP hands out a whole new lease/room.
  - THINK HOTEL
  
  
 # DHCP Continued 
 - Scope: You can specify the IP address range you would like DHCP to supply or prohibit from clients
  1. 192.168.1.100 - 200
 - Exclusions - Admins can have DHCP exclude specific ranges from clients
  2. 192.168.1.105 - 110 
 - Reservations - 192.168.1.10 for 1F-B8-DD-92-5A-5F
  3. Based on MAC addresses


# Static IP Address
- To understand DHCP, one must understand Static IP address.
- Static IP addresses are manually assigned by an admin. Does not change.


# DORA
- Client sends DHCP Discover to entire network
- DHCP server responds with an DHCP offer 
- Client requests offered settings
- DHCP server sends acknowledgements
  
# Why use Static IPs?
- Well our DNS server needs a static IP - where it does not change
- What if DNS server uses DHCP and IP change every week?
- If DNS server uses DHCP, then we would need to update our DHCP settings with a new IP address each time. It's too complicated thats why DNS ssrvers have static IP!
- Servers that provides services like DNS servers use static IPs
- Printers or scanners use static IPs - so we don't need to enter their IP each time. It's more convenient.
- If DHCP server crashes, then computers will lose their DHCP IP address - which is why static IP may work.
  
  
# DHCP Server Role enables the DHCP Network Protocol!!!!


  
# Add the DHCP Server Role to the Domain Controller (KevinVM)
 
 <p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/176341597-1fbbfe8b-83c2-433f-bd24-0b09c8397e52.png" height="175%" width="175%" alt="AD DS"/>
  
<p/>

  
# After installing DHCP, click the "Complete DHCP Configuration"
- You wll be prompted to create 
  1. DHCP Admins
  2. DHCP Users

# By default, this username will be generated. Click commit.
 <p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/176342312-9f0e7b21-490e-4bdd-ac74-b10c51695189.png" height="100%" width="100%" alt="AD DS"/>
  
<p/>
