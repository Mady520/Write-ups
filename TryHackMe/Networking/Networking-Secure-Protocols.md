## Networking Secure Protocol - TryHackMe  

### Overview  
This room teaches about the securing protocols like SSL/TLS ,how to secure existing protocols  
HTTP, POP3, SMTP, IMAP and how SSH replaced the plaintext TELNET.  

### Concepts  

**TLS**
Transport layer security is added to existing protocols to protect communication , confidentiality,integrity and authenticity .Consequently HTTP ,POP3 ,SMTP and IMAP become HTTPS, SMTPS,POP3S,IMAPS, where the appended S stands for Security.  

It is deemed insecure to remotely access a system using the TELNET protocol; Secure Shell (SSH) was created to provide a secure way to access remote system.
like SSL ,its predecessor ,TLS is a cryptographic protocol operating at the OSI model's transport layer. It allows secure communication between a client and a server over an insecure network. By secure we refer to Confidentiality & Intergrity. TLS ensures that no one can read or modiy the exchanged data.  

**HTTPS over TLS**  
`HTTPS` &rarr; Hypertext transfer protoccol Secure. It is basically `HTTP` over `TLS`. Consquently requesting a page over HTTPS will require the following steps:  

- Establish a TCP-Three way handshake with the target server.  
- Establish a TLS session.
- Communicate using the HTTP protocol.
- Getting the Encryption key.
- Adding TLS to HTTP leads to all packets being encrypted.

The key takeaway is that TLS offered security for HTTP without requiring any changes in the lower or higher layer protocols.  

**OpenSSH** offers several benefits:  
- Secure authentication.
- Confidentiality.
- Integrity.
- Tunnelling.

**SFTP** stands for SSH file transfer protocol  and allows secure file transfer.Part of SSH protocol suite and shares the same port no. 22.   
**FTPS** File transfer protocol secure, it is secured using TLS , usually uses port 990.   


          
