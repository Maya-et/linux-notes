# Linux Course Notes

Notes and exercises from my Kali Linux course.

## 1. Windows vs Kali Linux
windows is general purpose os and also its widely used os. it developed (owned) by Microsoft and not an open source which means we have to pay to get license 
kali linux is an open source or free. built for penetration testing, professionals and any one( hobbyist) can use it but it target cybersecurity professionals 
## 2. Linux File Hierarchy & Structure
unlike window which use drives (C, D) linux put everything under single organized file hierarchy which starts with single root directory represented by forward slash / to the top and everything else included under this root
/ is root of entire file system
/bin is user command binaries like ls,cd,cat
/etc is for system wise configuration files
/home is directories for regular users.
/root is directory for the root superuser.
/var  is Log, spool, and highly dynamic files.

## 3. Text Editors: nano vs vim
nano is simple and modaless. u can write anything u want write away its good for quick result also its user friendly some commands to save file we use ctrl + o and ctrl + x to exit or quit
vim is advanced model editor required learning keyboard shortcut. its good for complex navigation we use :w to save file and :q or :wq (save & quit)
## 4. Linux User Management
a core system administration task that controls system access, sets up security boundaries, and assigns resource permissions across multi-user environments. 
Root (Superuser)	Full system control. Can install software, change config files, and delete anything. Powerful but risky.
Regular User	Limited access. Can create files, run applications, but not modify system-level settings.
Sudo User	Regular user with temporary admin rights via the sudo command. Common in modern systems.
## 5. Package Installation (apt, pacman)
unlike os like windows that we install .exe files in linux software is bandled into package. package manager will download the requested software and install it for us all from terminal and also it manages dependencies which means like if the app requires any library it notices and download it for us.
apt( stands for advanced package tools) used for Ubuntu, Debian, Linux Mint Software files for these systems end in .deb. apt acts as the middleman between our command line and Ubuntu/Debian servers. Before installing anything, we run apt update so our computer fetches the latest list of available apps and versions. When we run apt install, it grabs the .deb file, unpacks it, places the files in the right system directories, and configures them.
pacman( stands for Package Manager Utility) used for Arch Linux, Manjaro unlike debian/ubuntu it uses rolling release model (constantly updating everything). and its built for extremely fast and lightweight also uses single letter flags like -s for Sync/Install
pkg (stands for Package.) and its used on Termux (the Linux terminal environment on Android smartphones) and FreeBSD.its design us simplified user freindly script
so in short Linux distributions use different tools depending on their architecture
## 6. Script Installation
insted of downloading a pre compiled package file script installation download text file containing  a sequence of terminal commands also unlike other file they cannot run unless they have given execute permission via chmod +x. and they required interpreter to red and excute their commands line by line

## 7. Software Installation Methods


## Basic Commands Practiced

- `mkdir` — (Make Directory) this command used for to create new , empty folder
  example   mkdir marta create folder name marta
- `cd` — (change directory) move u from current folder to other
  example  cd marta moves me to marta folder
- `ls -la` — (List All Files with Details) list every file and folder inside ur current directory
- `cat` — (View File Content) display the entire text contents of a file
- `mv` — (Move / Rename)  move file into another directory or rename
- `rm` — (Remove): Deletes files permanently.
- `echo` — (Print Text) display line of text or write text directly into file when paired with redirect ( > )
- `nano` — (Text Editor) Opens a simple, terminal-based text editor used to write or modify plain text files.

MASTERING THE POWER
USER TOOLS 
1.sudo 
2.grep 
3.find
4.chmode 
5,ps & top 
6.strings


## Task 2: File Practice

- Created `zxc.txt` with a short paragraph
- Counted word occurrences with `grep -oi`
- Counted total words with `wc -w`
