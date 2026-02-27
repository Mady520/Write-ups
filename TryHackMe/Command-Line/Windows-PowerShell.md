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
`get-location` &rarr; changes the current working directory and also tells the current working directory.  
`get-command ` To list all avaliable cmdlets functions , aliases and scripts that can be executed in the current PowerShell session.  
`get-help` Provides detailed information about the cmdlets, including usage ,parameters and examples.  
