## Windows fundamentals 1 - TryHackMe

### Overview
This room provided fundational knowledge of  the Windows operating system, giving small intro about the past windows and currently windows systems , Remote Desktop Protocol, file system , Different users , system configuration files etc.  
Windows is one of the most used operating system ,proprietary GUI-based operating system developed by Microsoft, commanding over 90% of the PC market.  

### Concepts learned  
Windows 11 pro has `bitlocker` encryption as compared to the normal windows home.  

`RDP Protocol` provides remote display and input capabilities over netwrok connections for windows-based applications running on server.  
for using `RDP` we should have :  
`MACHINE IP` &rarr; remote machine.  
`user/username` and `password`.  

In modern windows there is `NTFS` file system *NEW TECHNOLOGY FILE SYSTEM* it is the primary file system for Windows, offering superior reliability, security, and capacity compared to older formats like FAT32/FAT16. Key advantages include support for massive file/volume sizes (up to 16 exabytes), journaling for fast data recovery, file-level encryption (EFS), compression, and advanced user permissions.  
using `NTFS` we can set permissions on files and folders.  
**Permissions** are:  
- Full control  
- Modify
- Read & execute
- List folder content
- Read
- Write

`system32` traditionally known as the folder whihc contains the windows operating system. It holds the important files that are critical for the operating system.  
`%windir%` &rarr; system environment variable directory for windows. Environment variables store information about the operating system environement. The informaiton includes such as OS path , the number of processors used by OS, and the location of temporary files.  

**Administrator**   
      &darr;       
 can do anything. Can add , delete users , can modify groups ,can change any setting in the system.  
   
 **Standard User**  
       &darr;  
Makes chnages only to folders & files , can't perform system-level changes.  

User Account Control `UAC` &rarr; a mandatory security feature in Microsoft Windows designed to prevent unauthorized, potentially malicious changes to the operating system. It acts as a gatekeeper, prompting for permission or an admin password before allowing tasks that require administrative privileges, such as installing software or modifying system settings.  
