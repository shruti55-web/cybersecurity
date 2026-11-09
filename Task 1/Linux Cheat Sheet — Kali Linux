1. Basic navigation
Command	Use
pwd	Show current directory
ls	List files
ls -la	List all files, including hidden files
cd folder	Enter a directory
cd ..	Go to parent directory
cd ~	Go to home directory
clear	Clear terminal display
history	View command history

2. File and directory management
Command	Use
mkdir lab	Create a directory
mkdir -p a/b	Create nested directories
touch file.txt	Create an empty file
cat file.txt	Display file contents
nano file.txt	Edit a text file
cp a.txt b.txt	Copy a file
mv old.txt new.txt	Rename or move a file
rm file.txt	Delete a file
find . -name "*.txt"	Find text files
file filename	Identify file type

Be careful with rm, particularly when using recursive or force options.
3. Permissions and users
Command	Use
whoami	Show current username
id	Show user and group IDs
sudo command	Run a command with elevated privileges
chmod +x script.sh	Make a script executable
chmod 600 file.txt	Give the owner read/write access only
chown user file.txt	Change file ownership, with appropriate privileges

Linux permissions use r for read, w for write, and x for execute.
4. System information and processes
Command	Use
uname -a	Show kernel and system details
cat /etc/os-release	Show Linux distribution details
df -h	Check disk space
free -h	Check memory usage
ps aux	List running processes
top	Monitor processes
kill PID	Send a signal to a process
uptime	Show system uptime

5. Networking commands
Command	Use
ip -br addr	Show interfaces and IP addresses
ip route	Show routing table
ping -c 4 1.1.1.1	Test IP reachability
ss -tuln	Show listening TCP/UDP sockets
nslookup example.com	Perform DNS lookup
dig example.com	Query DNS records
curl -I https://example.com	Request HTTP response headers
traceroute example.com	Trace network path, if installed
sudo tcpdump -i any	Capture packets on available interfaces

6. Package management
Command	Use
sudo apt update	Refresh package lists
sudo apt upgrade	Upgrade installed packages
sudo apt install nmap	Install Nmap
sudo apt install wireshark	Install Wireshark
sudo apt install netcat-openbsd	Install Netcat implementation
sudo apt remove package	Remove a package

7. Text searching and hashing
Command	Use
grep "error" file.txt	Search for text
wc -l file.txt	Count lines
sort file.txt	Sort lines
sha256sum file.txt	Calculate SHA-256 digest
md5sum file.txt	Calculate MD5 digest
openssl dgst -sha256 file.txt	Calculate SHA-256 using OpenSSL

8. OpenSSL quick reference
Command	Use
openssl version	Check OpenSSL version
openssl rand -hex 16	Generate 16 random bytes in hexadecimal
openssl dgst -sha256 file.txt	Calculate a SHA-256 digest
openssl enc -aes-256-cbc -salt -pbkdf2 -in in.txt -out out.bin	Encrypt a file
openssl enc -d -aes-256-cbc -pbkdf2 -in out.bin -out recovered.txt	Decrypt a file