## Linux-Fundamentals-2 

### Overview 
This room provided the fundational knowledge of the Linux operating system ,focusing on the command line usage, file system navigation , file permissions,accessing linux machine remotely using SSH protocol , knowing about some important files of the Linux operating system and also about creating , copying and moving files/folders.  

### Command practiced  
```bash
SSH
```
Usage
```bash
ssh username@IP
```
**Secure shell** --> used for connecting and interacting with the command line of a remote linux machine or it is used to connect to a remote linux machine.  
Can access Linux machine remotely bby knowing the ip and login credentials.  

### Commands practiced  
```bash
ls
ls --help
man ls
ls -h
touch
mkdir
cp
mv
rm
file
rm -R
```
### Concepts learned 
- Listing files/folder.  
- Listing in human readable format.
- Knowing manual/documentation of a command.
- Create files.
- Create , Copy , Move a file/folder.
- Remove a file/folder/directory.
- Know rhe file type of a file.

### Permission commands  
**ls -l** shows files/folders with permissions.  
Read &rarr; r &rarr; 4  
Write &rarr; w &rarr; 2  
Execute &rarr; x &rarr; 1  

rwxrwxrwx &rarr; First rwx is of owner , next rwx is of group , last rwx is of others.  
The permissions are kept by, what can owner do , what can group do and what can others do to a file. The one who has rwx all that measn that onwer/group/other can read write and execute all three to the file having rwx. If all have *rwxrwxrwx* then the value is 777.  

### Commands    
```bash
chmod 777
chmod 756
Su
```
### Concepts learned 
- File permissions.
- Know how to change the permissions.
- Switching users by using *su* command.


  




