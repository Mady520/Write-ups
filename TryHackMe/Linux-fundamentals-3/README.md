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
- User if the remote machine.
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
