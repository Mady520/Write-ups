## Linux Fundamentals 3 - TryHackMe

### Overview 
This room provided with the Linux fundamentals, focused on command line usage , introduction to text editors, downloading files from web , copying files between two computers remotely, introduction of server , process management , checking , enabling , disabling processes , scheduling processes, adding additional repositories to your OS.  

### Commands Practiced  
```bash
nano
vim
wget
scp
pyhton3 -m http.server
```
### Concepts learned 
`nano` and `vim` are text editors while `vim` is more advanced then `nano`  
`wget` is used to download files from the web via http.  
`scp` used during ssh to copy files between two computers remotely.  
For `scp` several information is needed  
- Ip address of remote machine.
- User of the remote machine.
- Name of the file on the local system.
- Name we wish to store the file as on the remote system.
e.g `scp file.txt ubuntu@IP:/home/ubuntu/filecopied.txt`.

### Commands Practiced
```bash
ps
ps aux
ps aux --sort-%CPU
top
kill pid
SIGTERM
SIGKILL
SIGSTOP
systemctl
fg
cron
```
### Concepts 
`python3 -m http.server` is used to create a local server (if needed for some projects/work).  
`updog` &arr; advanced server.  
`pid` &arr; Process ID.  
`ps` &arr; Provides list of the running processes, user's session and some additional information.  
`ps aux --sort-%CPU` &arr; Shows resource heavy processes running.  
`kill pid` &arr; To kill a process.  
`SIGTERM` &arr; Kill the process, but allows it to do some cleanup beforehand.  
`SIGKILL` &arr; Kill the process,doesn't do any cleanup after the fact.  
`SIGSTOP` &arr; Stop/suspend a process.  
`systemctl` &arr; This command allows us to interact with the systemmd processes/deamon.  
`fg` &arr; used to bring background processes into use on the terminal, where the output of the script is now returned to us.  
`crontab` &arr; one of the processes that is started during boot, whihc is responsible for facilitating and managing cron jobs.  
`dpkg` &arr; Package installers.  


