## Windows PowerShell - TryHackMe

### Overview
This room gave the knowldege about the Windows Powershell , its basics ,and the basic commands , It also gave introductory to the piping term and how that is used.  

### Concepts Learned 

**PowerShell** &rarr; It is a powerful tool from Microsoft designed for task automation and configuration management. It combines a command-line interface and a scripting language built on `.NET` framework. PowerShell is object-oriented , which means it can handle complex data types and interact with the system componets more effectively.  

### PowerShell Basics  
```bash
commandlets /cmdlets                                      aliases
get-content                                               dir 
get-location                                              cd
get-command                                               -path
get-command -commandtype -function                        new-item 
get-help                                                  remove-item
copy-item                                                 move-item
```

`commandlets` &rarr; PowerShell commands are known as commandlets. These are much more powerful then the traditional windows commands and allow for more advanced data manipulation.
`get-content` &rarr; Retrieves the content of a file an displays it inot console.  
`get-location` &rarr; Changes the current working directory and also tells the current working directory.  
`get-command` &rarr; To list all avaliable cmdlets functions , aliases and scripts that can be executed in the current PowerShell session.  
`get-help` &rarr; Provides detailed information about the cmdlets, including usage ,parameters and examples.  
`dir` &rarr; Lists the files and directories in a location specified.  
`Aliases` &rarr; Shortcuts or alternnative names for cmdlets , e.g cd == set-location.  
`new-item` &rarr; To create an item in PowerShell. 
`remove-item` &rarr; Removes both files and directories.  
`copy-item` &rarr; Copies the files.  
`move-item` &rarr; Equivalent to move. 

### Piping  
It is a technique in command-line environment that allows the output of one command to be used as the input for another command.
E.g : ```  get-childitem |Sort-object length. ``` 
Will display the contents then sort them according their lengths.  

```bash
get-childitem                                         get-netipaddress
select-object                                         get-process
select-string                                         get-service
get-computerinfo                                      get-nettcpconnection
get-localuser                                         get-filehash
ipconfig                                              get-netipconfiguration
```

`get-childitem` &rarr; Display the contents of a file or directory.  
`select-object` &rarr; It is a filtering cmdlets. Used to specify properties from objects or limit the number of object returned.  
`get-computerinfo` &rarr; Retrieves comprehensive system information, including OS info , hardware specification BIOS details and more.  
`get-localuser` &rarr; Lists all the local user accounts on the system.  
`ipconfig` &rarr; Retrieve info. about the system's network configuration.  
`get-netipconfiguration` &rarr; Provides detailed information about the network interfaces on the system , including IP addresses, DNS servers, and gateway configuration.  
`get-netipaddress` &rarr; Will show details of the ip address configured on the system.  
`get-process` &rarr; provides a detailed view of all currently ruuning process, including CPU and memory usage , making it powerful tool for monitoring and troubleshooting.  
`get-service` &rarr; Allows the retrieval of information about the status of services on the machine , such as which service is running , stopped or paused.   
`get-nettcpconnection` &rarr; Displays current TCP connections, giving insights into both local and remote endpoints.  
`get-filehash` &rarr; For Displaying the file hashes.  

**Scripting** &rarr; Process of writing and executing a series of commands contained in a text file known as script,  to automate tasks that one would generally perform manually in a shell.  






