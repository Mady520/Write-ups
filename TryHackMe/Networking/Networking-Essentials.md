## Networking Essentials - TryHackMe

### Overview
This room teaches about various standard protocols and technologies that glue things together.  
Dynammic Host Configuration Protocol (DHCP)    
Address resolution Protocol (ARP)    
Network Address Translation (NAT)    
Internet Control Message Protocol (ICMP)  


### Concepts   
Whenever we want to access a network, at the very least, we need to configure the following:  
IP address along with subnet mask.  
Router (or Gateway)  
DNS server.  
Having an automated way to configure connected devices has many advantages. This solution lies in `DHCP`.  
`DHCP` is an applicatoin protocol that relies on `UDP`, the server listens on `UDP` port 67 and client sends from `UDP` Port 68.  

`DHCP` follows `DORA`  
`D` Discover   
`O` Offer  
`R` Request  
`A` Acknowledge  

**Address Resolution Protocol** `ARP` &rarr; makes possible to find the MAC address of another devices on the Ethernet. An ARP request or ARP reply is not encapsulated within a UDP or even IP packet , it is encapsulated directly within an Ethernet frame.  

**Internet Control Message Protocol** `ICMP` &rarr; is maninly used for network diagnoses and error reporting. Two popular commands reply on ICMP and they are instrumental in network troubleshooting and network security.  
|--`Ping` This command uses `ICMP` to test connectivity to a target system and measures the round-trip-time (RTT).    
|--`Tracert` It uses `ICMP` to discover the route from your host to the target.  

**Routing** &rarr; Selecting optimal path for data packets across networks. Operates at level 3. Routing algo's --> OSPF ,BGP, EIGRP, RIP.  

**Network Address Translation**`NAT` &rarr; Solution to depletion of addresses. The idea behind NAT lies in using one public address IP address to provide inernet access to many private IP addresses. NAT supporting routers maintain a table translating network addresses betwenn internal and external networks.  

