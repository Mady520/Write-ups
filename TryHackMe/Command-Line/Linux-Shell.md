## Linux-Shell - TryHackMe

### Overview
This room gives the basic knowledge of the Linux Shell. Learn interaction with Linux Shell , using basic commands ,explore the types of Linux Shells available and introduction to shell scripting.  

Most Linux distribution uses Bash(Bourne again shell) as their default shell.  

### Commands 
```bash
pwd                          grep       
cd                           cat
ls                           echo $shell
cat /etc/shells                        
```

### Concepts learned 
`pwd` &rarr; Print working directory.  
`cd` &rarr; Change directory.  
`ls` &rarr; List contents of a file.  
`grep` &rarr; Used to search for any word or pattern inside a file.  
`echo $shell` &rarr; To know which shell is being used.  
`cat /etc/shells` &rarr; To list down all shells in your linux.  

There are different types of shells in linux , the default is Bash shell, full form as Bourne again shell ,also there are Zsh shell ( Z shell ) and Fish (friendly interactive Shell).  

*Bourne again shell* &rarr; offers widely compatible scripting with extensive documentation available. It allows the basic customization and in this shell the Syntax highlighting is not available.  

*Zsh* &rarr; Offers excellent level of scripting and it has some extra features then *Bash* , it allows advanced customization and it has built-in Syntax highlighting.

*Fish* &rarr; Offers limited scripting and does not contain that much features ,offers good customization more then *Bash* but less then *Zsh* and it has syntax highlighting  available  in some plugins.  

**Shell Scripting** &rarr; Nothing but set of commands. Scripting helps us to automate tasks making time usable more. Scripting can be done in various programming languages as well.  The default extension for *Bash* is `.sh`.  

Example of a script asking name!  
```bash
#!/bin/bash
echo "Hey, What is your name!"
read name
echo "Welcome, $name"
```
output 
```bash
Hey , What is your name!
john                         ---> user typed
Welcome, john
```




