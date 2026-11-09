Wireshark — Packet Capture

Purpose: Capture and analyze network packets.

Useful display filters:
Filter	Purpose
dns	DNS traffic
icmp	Ping traffic
tcp	TCP packets
tls	TLS records
http	Identified HTTP traffic

Generate test traffic:
ping -c 4 1.1.1.1
nslookup example.com
curl -I https://example.com


Start capturing on the interface carrying the traffic, inspect packet details, stop the capture, and save it as wireshark-test.pcapng. Only capture traffic you are authorized to inspect.

Nmap — Network Scanning

Purpose: Discover hosts, ports, and services on authorized systems.
nmap -sn 192.168.1.0/24
nmap -sS <authorized-target>
nmap -sV <authorized-target>
nmap -sU <authorized-target>


- -sn: Host discovery without port scanning.
- -sS: TCP SYN scan.
- -sV: Service version detection.
- -sU: UDP scan.
Replace placeholders with systems in your own lab or systems you have explicit permission to test.

Burp Suite — Web Proxy

Purpose: Inspect and test HTTP/HTTPS requests and responses in web applications.

Main features:
- Proxy: Intercepts and inspects browser traffic.
- Repeater: Manually modifies and resends requests.
- Intruder: Automates customized request testing.
- HTTP history: Reviews captured requests and responses.
Practice on a deliberately vulnerable local application or an authorized training environment.

Netcat (nc) — Network Debugging

Purpose: Make TCP/UDP connections and help troubleshoot network services.
nc -h
nc -vz <authorized-host> 80
nc -vz <authorized-host> 443


- -v: Verbose output.
- -z: Check connection without sending application data.
Netcat can be used as a basic connectivity test, but the exact options vary between implementations.