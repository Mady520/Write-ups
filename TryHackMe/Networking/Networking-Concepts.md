## Networking Concepts - TryHackMe

### Overview
This room introduces to the vital networking concepts and the most common networking protocols. Gives introduction about ISO OSI network model, IP adresses, subnets, and routing, TCP, UDP & port numbers, how to connect to an open TCP port from the commmand line.  

### Concepts 
**OSI** (Open System Interconnection) model is a conceptual model developedd by the International Organisation for Standardization (ISO) that describes how communication should be occur in a computer network. OSI model defines a framework for computer network communications.  

The OSI model is composed of 7 seven layers:  
1. Physcical layer
2. Data link layer
3. Network layer
4. Transport layer
5. Session layer
6. Presentation layer
7. Application layer

**Physcial layer** &rarr; Physical data transmision media. Electrical ,optical and wireless signals.
**Data link layer** &rarr; Reliable data transfer between adjacents , error control and flow control. Ethernet (802.3), WI-Fi (803.11).  
**Network layer** &rarr; Logical addressing and routing between networks. IP, ICMP ,IPsec.  
**Transport layer** &rarr; End to end communication and data segmentation. Ports UDP,TCP.
**Session layer** &rarr; Establishing ,mainintaing connections and data segmentation.NFS, RPC.  
**Presentation layer** &rarr; Data encoding - decoding, encryption and compression. MIME, JPG ,PNG, MPEG.  
**Application layer** &rarr; Provides services and interface to application. HTTP, FTP,DNS,POPS,SMTP,IMAP.  

### TCP/IP Model 
Implemented model  
Transmission Control Protocol/ Internet protocol was developed in the 1970's by the department of defenses DOD.  
```bash
      **TCP/IP**              ------------------------->          **OSI**  
     _____________________                                  ________________________
    |                     |                                |Application layer       |  
    | Application layer   |    ------------------------->  |Presentation layer      |  
    |                     |                                |Session layer           |  
    |---------------------|                                |------------------------|
    | Transport layer     |  ----------------------->      | Transport layer        |                                                   
    |                     |                                |                        |
    |---------------------|                                |------------------------|                                                     
    | Internet layer      |  ------------------------>     |  Network layer         |
    |                     |                                |                        |
    |---------------------|                                |------------------------|
    |                     |                                |   Data link layer      |
    |  Link layer         |  ------------------------->    |                        |
    |_____________________|                                |   Physical layer       |
                                                           | ______________________ |
    
```

Each host on the network needds a unique identifier for other hosts to communicate with him without a unique identifier , the host cannot be found.  
That is why IP address was introduced . `IPv4` and `IPv6`.  

A router forwards data packets to the proper network, usually a data packet passes through multiple routers before it reaches its final destination the router functions at layer 3, inspecting the ip address and forwarding the packet to the best network (router) so the packet gets closer to its destination.  

