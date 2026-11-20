Linux is an open-source operating system widely used for servers, cloud infrastructure, networking, and cybersecurity.

Kali Linux is a Debian-based distribution containing tools for security testing and digital forensics.
Basic Linux commands
Command	Purpose
pwd	            Display the current directory
ls -la	        List files, including hidden files
cd /path	    Change directory
mkdir lab	    Create a directory
touch file.txt	Create an empty file
cat file.txt	Display file contents
nano file.txt	Edit a text file
cp a.txt b.txt	Copy a file
mv a.txt b.txt	Move or rename a file
rm file.txt	    Delete a file
whoami	        Display current username
sudo command	Execute a command with elevated privileges

Linux file system
- / — Root directory.
- /home — Users' personal directories.
- /etc — System configuration files.
- /var — Variable data, including many logs.
- /tmp — Temporary files.
- /root — Home directory of the root user.
- /usr/bin — Common user commands and executable programs.
File permissions
Linux permissions define who can read, write, or execute a file.
- r — Read
- w — Write
- x — Execute
Example:
ls -l
chmod 600 file.txt
chmod +x script.sh


chmod 600 file.txt gives the owner read/write permission and removes permissions for group and others.
Package management in Kali Linux
sudo apt update
sudo apt upgrade
sudo apt install nmap


- apt update refreshes package lists.
- apt upgrade upgrades installed packages.
- apt install installs a package.
Processes and system monitoring
ps aux
top
free -h
df -h


These commands help inspect running processes, memory usage, and disk space.
Linux networking
ip addr
ip route
ping -c 4 1.1.1.1
ss -tuln


These commands show network addresses, routes, connectivity, and listening TCP/UDP ports.