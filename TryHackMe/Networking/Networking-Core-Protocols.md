## Network Core Protocols - TryHackMe  

### Overview
This room teaches about he networking core protocols on which the network works. Will get the knowledge about the following:  
Whois  
DNS  
HTTP & FTP  
SMTP , POP3 & IMAP  

### Concepts
**DNS**  
`DNS` &rarr; Domain Name System,  which is responsible for properly mapping a domain name to an IP address. It operates at application layer. DNS traffic uses `UDP` port 53 by default and `TCP` port 53 as a default feedback.  

**DNS Records**  
`A record` &rarr; A address maps a hostname to one or more IPv4 addresses.  
`AAAA record` &rarr; The AAAA recored is similar to the A record but it is for IPv6.  
`CNAME` &rarr; The CNAME (Conanical record) maps a domain name to another domain name.  
`MX record` &rarr; The Mx (Mail Exchange) record specifies the mail server responsible for handling emails for a domain.  

Someone needs the authority to set A , AAAA records & Mx records among other DNS record for the domain. Whoever registers a domain name is granted this power.
Therefore, that can set any valid DNS record.This information is part of data available via `WHOis` records and is available publicly.  

**HTTPS**  
`HTTPS/HTTP`  &rarr; Hypertext Transfer Protocol, the S stands for Secure. This protocol relies on TCP & defines how your web browser communicates with the web server.  
   **Common Commands**  
   `GET` &rarr; Retrieves data from a server , such as an HTML file , or an image.  
   `POST` &rarr; Allows us to submit new data to the server. e.g submitting a form.  
   `PUT` &rarr; Is used to create a new resource on the server and to update and overwrite existing information.  
   `DELETE` &rarr; Is used to delete a specified file or resource on the server.  
**Using `TELNET` and using `GET` to get a file:**  
```bash
Telnet IP PORT  
GET file.txt HTTP/1.1  
HOST: anything
```

**FTP**  
is designed to transfer files. `FTP` is very efficient for file transfer and when all conditions are equal ,it can achieve higher sppeds then `HTTPS`.  
Common options:  
`USER` &rarr; Input the username.  
`Pass` &rarr; Input for password.  
`RETR` &rarr; Retrieve/download a file from http.  
`STOR` &rarr; Upload a file from client to FTP server.  
**Example**
```bash
FTP <IP>
User -----
Pass -----
get filename --> to download.
```

**SMTP**   
Simple Mail Tranfer Protocol, defines how a mail client talks with a mail server and how a mail server talks with another.  
`HELO` &rarr; Initiates an SMTP session.  
`MAIl from` &rarr; Sender's mail address.  
`RCPT to` &rarr; Reciepts mail address.  
`DATA` &rarr; Will begin to sending the contents of the email message.  
`.` &rarr; To indicate end of message.  

**POP3**   
Post Office Protocol Version 3 &rarr; is designed to allow client to commnicate with a mail server and retrieve email message.
`USER` &rarr; Username.  
`PASS` &rarr; Password.  
`STAT` &rarr; Request the number of messages and total size.  
`LIST` &rarr; List all messages and their size.  
`RETR` &rarr; Retrives messages.  
`DELE` &rarr; Marks a message for deletion.  
`QUIT` &rarr; Quits.  

**IMAP**   
Allows synchronizing read , moved and deleted messages. IMAP is quite convenient when you check your email via multiple clients. IMAP tends to use more storage as email is kept on the server  and synchronise across the email client. 
`LOGIN` &rarr; <username> <password>.  
`SELECT <mailbox>` &rarr; Select mailbox.  
`FETCH <mailno> <data item no>`.  
`MOVE <Sequence set> <mail box>`  
`COPY <sequence set> <data item name>`  
`LOGOUT`.





