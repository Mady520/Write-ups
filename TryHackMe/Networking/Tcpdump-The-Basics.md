## Tcpdump: The Basics - TryHackMe  

### Overview  
This room introduces some basic command-line arguments for using Tcpdump. The Tcpdump tool and its libpcap library are written in c and c++ and were released for Unix-like systems in the late 1980's.They are very stable and offer optimal speed.The libpcap library is the foundation fro various other networking tools today, it was ported to Windows as Winpcap.  

### Concepts   

### TcpDump   
Tcpdump is a powerful command-line packet analyzer used to capture, filter, and analyze network traffic in real-time or save it to a file.  
```bash
tcpdump -i                                   tcpdump -v  
tcpdump -i any
tcpdump -i eth0
tcpdump -w file.pcap
tcpdump -r file.pcap
```
`-i` &rarr; interface &rarr; to specify one interface network to listen to.   
`-i any` &rarr; To listen on all available interfaces.  
`-i eth0` &rarr; Specified network interface.  
`-w` &rarr; for saving captured packets in a file.  
`-r` &rarr; For reading packets from a file.  
`-c` &rarr; To specify the no of packets to capture.  
`-v` &rarr; FOr verbose output.  

Tcpdump will resolve IP addresses and print friendly domain names where possible, to avoid making such DNS lookup, `-n ` argument is used , Similarly if you dont want the port no to be resolved `-nn` is used to stop both DNS and PORT no lookup.  



