## Windows Command Line - TryHackMe

### Overview 
This room taught how to use MS Windows Command prompt `cmd.exe`.The default command line interpreter in the Windows environment.It taught about its advantages sucha s fast, efficient ,lower memory usage ,remote management ,and automation.  

### Commands Practiced
```bash
Set command                     type
ver                             rmdir
systeminfo                      mkdir
help                            tree
cls                             dir
ipconfig                        dir /a
ipconfig /all                   cd
ping                            copy
tracert                         move
nslookup                        del or erase
netstat                         tasklist
taskkill pid                    chkdsk
drivequery                      shutdown /?
```

### Concepts 
`Set command` &rarr; To check your path from the command line.  
`ver` &rarr; To determine the OS version.  
`systeminfo` &rarr; To list various information about the system such as Operating system information ,system details , processor and memory.  
`help` &rarr; Provides help info for a specfic command.  
`cls` &rarr; Clears the command prompt screen.  
`dir` &rarr; Used to view th child directories.  
`dir /a` &rarr; Displays hidden and system files as well.  
`tree` &rarr; Visually represent the child directories & subdirectories.  
`mkdir` &rarr; Make directory.  
`rmdir` &rarr; Remove directory.  
`type` &rarr; View easily tet files.  
`copy` &rarr; Allows to copy file from one location to another.  
`del or erase` &rarr; Delete a file.  
`tasklist` &rarr; Lists the running processes.  
`taskkill pid` &rarr; To kill a process.  
`Chkdsk` &rarr; Checks file system and disk volumes for errors and bad sectors.  
`drivequery` &rarr; Displays a list of installed device drivers.  


### Network-commands  
`ipconfig` Network information.  
`ipconfig /all` For more information about your network configuration.  
`ping` One common troubleshooting task is checking if the server can access a particuler server on the Internet.  
`tracert` Trace route , traces the network route traversed to reach the target without getting into more details, it expects the routers on the path to notify us if they drop packet because its Time To Live (TTL) has reached zero.  
`nslookup` It looks up a host or domain and returns its IP address.  
`netstat` Displays current network connections and listening ports.  
`netstat -abon` Gives fully information about what is listening or which process is running.  







