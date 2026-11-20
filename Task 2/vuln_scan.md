live hosts
# Nmap 7.99 scan initiated Mon Nov  9 09:33:54 2026 as: /usr/lib/nmap/nmap -sn -oA 01_host_discovery 192.168.1.3/24
Host: 192.168.1.1 ()	Status: Up
Host: 192.168.1.2 ()	Status: Up
Host: 192.168.1.3 ()	Status: Up
Host: 192.168.1.4 ()	Status: Up
# Nmap done at Mon Nov  9 09:33:57 2026 -- 256 IP addresses (4 hosts up) scanned in 3.10 seconds


# 2. TCP SYN scan, all ports
# Nmap 7.99 scan initiated Mon Nov  9 09:36:11 2026 as: /usr/lib/nmap/nmap -sS -p- -oA 02_tcp_syn 192.168.1.3
Nmap scan report for 192.168.1.3
Host is up (0.00025s latency).
Not shown: 65505 closed tcp ports (reset)
PORT      STATE SERVICE
21/tcp    open  ftp
22/tcp    open  ssh
23/tcp    open  telnet
25/tcp    open  smtp
53/tcp    open  domain
80/tcp    open  http
111/tcp   open  rpcbind
139/tcp   open  netbios-ssn
445/tcp   open  microsoft-ds
512/tcp   open  exec
513/tcp   open  login
514/tcp   open  shell
1099/tcp  open  rmiregistry
1524/tcp  open  ingreslock
2049/tcp  open  nfs
2121/tcp  open  ccproxy-ftp
3306/tcp  open  mysql
3632/tcp  open  distccd
5432/tcp  open  postgresql
5900/tcp  open  vnc
6000/tcp  open  X11
6667/tcp  open  irc
6697/tcp  open  ircs-u
8009/tcp  open  ajp13
8180/tcp  open  unknown
8787/tcp  open  msgsrvr
34346/tcp open  unknown
34850/tcp open  unknown
38090/tcp open  unknown
43300/tcp open  unknown
MAC Address: 08:00:27:62:6B:9F (Oracle VirtualBox virtual NIC)

# Nmap done at Mon Nov  9 09:36:13 2026 -- 1 IP address (1 host up) scanned in 2.32 seconds

# 3. UDP scan, top ports
# Nmap 7.99 scan initiated Mon Nov  9 09:37:06 2026 as: /usr/lib/nmap/nmap -sU --top-ports 100 -oA 03_udp -T5 192.168.1.3
Warning: 192.168.1.3 giving up on port because retransmission cap hit (2).
Nmap scan report for 192.168.1.3
Host is up (0.00048s latency).
Not shown: 88 open|filtered udp ports (no-response)
PORT      STATE  SERVICE
53/udp    open   domain
88/udp    closed kerberos-sec
111/udp   open   rpcbind
137/udp   open   netbios-ns
520/udp   closed route
998/udp   closed puparp
1434/udp  closed ms-sql-m
1719/udp  closed h323gatestat
2049/udp  open   nfs
32771/udp closed sometimes-rpc6
49181/udp closed unknown
65024/udp closed unknown
MAC Address: 08:00:27:62:6B:9F (Oracle VirtualBox virtual NIC)

# Nmap done at Mon Nov  9 09:37:11 2026 -- 1 IP address (1 host up) scanned in 5.03 seconds

# 4. Service version detection on open ports
 Nmap 7.99 scan initiated Mon Nov  9 09:37:57 2026 as: /usr/lib/nmap/nmap -sV -oA 04_versions 192.168.1.3
Nmap scan report for 192.168.1.3
Host is up (0.00015s latency).
Not shown: 977 closed tcp ports (reset)
PORT     STATE SERVICE     VERSION
21/tcp   open  ftp         vsftpd 2.3.4
22/tcp   open  ssh         OpenSSH 4.7p1 Debian 8ubuntu1 (protocol 2.0)
23/tcp   open  telnet      Linux telnetd
25/tcp   open  smtp        Postfix smtpd
53/tcp   open  domain      ISC BIND 9.4.2
80/tcp   open  http        Apache httpd 2.2.8 ((Ubuntu) DAV/2)
111/tcp  open  rpcbind     2 (RPC #100000)
139/tcp  open  netbios-ssn Samba smbd 3.X - 4.X (workgroup: WORKGROUP)
445/tcp  open  netbios-ssn Samba smbd 3.X - 4.X (workgroup: WORKGROUP)
512/tcp  open  exec        netkit-rsh rexecd
513/tcp  open  login       OpenBSD or Solaris rlogind
514/tcp  open  tcpwrapped
1099/tcp open  java-rmi    GNU Classpath grmiregistry
1524/tcp open  bindshell   Metasploitable root shell
2049/tcp open  nfs         2-4 (RPC #100003)
2121/tcp open  ftp         ProFTPD 1.3.1
3306/tcp open  mysql       MySQL 5.0.51a-3ubuntu5
5432/tcp open  postgresql  PostgreSQL DB 8.3.0 - 8.3.7
5900/tcp open  vnc         VNC (protocol 3.3)
6000/tcp open  X11         (access denied)
6667/tcp open  irc         UnrealIRCd
8009/tcp open  ajp13       Apache Jserv (Protocol v1.3)
8180/tcp open  http        Apache Tomcat/Coyote JSP engine 1.1
MAC Address: 08:00:27:62:6B:9F (Oracle VirtualBox virtual NIC)
Service Info: Hosts:  metasploitable.localdomain, irc.Metasploitable.LAN; OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Mon Nov  9 09:38:10 2026 -- 1 IP address (1 host up) scanned in 12.77 seconds

# 5. OS detection
# Nmap 7.99 scan initiated Mon Nov  9 09:38:24 2026 as: /usr/lib/nmap/nmap -O -oA 05_os 192.168.56.101
Host: 192.168.56.101 ()	Status: Up
Host: 192.168.56.101 ()	Ports: 	Ignored State: filtered (1000)
# Nmap done at Mon Nov  9 09:38:31 2026 -- 1 IP address (1 host up) scanned in 7.29 seconds

#6.Combined final scan
# Nmap 7.99 scan initiated Mon Nov  9 09:38:51 2026 as: /usr/lib/nmap/nmap -sS -sU -sV -O -p T:1-65535,U:53,69,111,123,137,161 -oA 06_full_scan 192.168.56.101
Nmap scan report for 192.168.56.101
Host is up (0.034s latency).
Not shown: 52582 filtered tcp ports (no-response), 12953 filtered tcp ports (net-unreach)
PORT    STATE         SERVICE    VERSION
53/udp  open|filtered domain
69/udp  open|filtered tftp
111/udp open|filtered rpcbind
123/udp open|filtered ntp
137/udp open|filtered netbios-ns
161/udp open|filtered snmp
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Aggressive OS guesses: 3Com 4500G switch (92%), H3C Comware 5.20 (92%), Huawei VRP 8.100 (92%), Microsoft Windows Server 2003 SP1 (92%), Oracle Virtualbox Slirp NAT bridge (92%), QEMU user mode network gateway (92%), AXIS 2100 Network Camera (92%), D-Link DP-300U, DP-G310, or Hamlet HPS01UU print server (92%), HP Tru64 UNIX 5.1A (92%), Sanyo PLC-XU88 digital video projector (92%)
No exact OS matches for host (test conditions non-ideal).

OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Mon Nov  9 09:44:14 2026 -- 1 IP address (1 host up) scanned in 323.31 seconds
