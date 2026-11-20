Cybersecurity is the practice of protecting computers, networks, applications, and data from unauthorized access, attacks, damage, and theft.

Key concepts
- Threat: Something that could cause harm to a system.
- Vulnerability: A weakness that an attacker could exploit.
- Exploit: A method or code that takes advantage of a vulnerability.
- Risk: The potential for loss or damage when a threat exploits a vulnerability.
- Attack vector: The path or method used to attack a system.
- Authentication: Verifying who a user is.
- Authorization: Determining what an authenticated user can access.
- Firewall: Filters network traffic according to security rules.
- MFA: Multi-factor authentication uses two or more different authentication factors
.
Common types of cyberattacks
Attack	                Meaning
Phishing	         Tricking users into revealing sensitive information
Malware              Malicious software
Ransomware           Malware that locks or encrypts data to demand payment
DDoS	             Overwhelming a service with traffic from multiple sources
SQL Injection	     Manipulating database queries through unsafe input
Brute Force        	Repeatedly trying credentials to guess a password

Types of cybersecurity
- Network Security
- Application Security
- Cloud Security
- Endpoint Security
- Information Security
- Identity and Access Management

2. CIA Triad — Core Security Principles
The CIA Triad represents three fundamental goals of information security.

C — Confidentiality

Ensures that information is accessible only to authorized people.

Example: Encrypting confidential files.


I — Integrity

Ensures that information remains accurate and is not changed without authorization.

Example: Using SHA-256 hashes to detect file changes.


A — Availability

Ensures that systems and information are accessible when needed.

Example: Maintaining backups and protecting servers against DDoS attacks.

 Confidentiality = secrecy; Integrity = accuracy; Availability = accessibility.
 
3. Cloud Environment Setup
Cloud computing provides computing resources such as servers, storage, networking, and software over the internet.

Cloud service models
Model	Description	Example
IaaS	Virtual machines, networks, and storage	AWS EC2
PaaS	Platform to build and deploy applications	Google App Engine
SaaS	Ready-to-use software over the internet	Microsoft 365

Cloud deployment models
- Public Cloud: Services provided over shared cloud infrastructure.
- Private Cloud: Cloud infrastructure dedicated to one organization.
- Hybrid Cloud: Combination of private and public cloud environments.
Basic cloud lab setup
1. Choose a cloud provider or a local virtual-machine environment.
2. Create an account or configure your local lab.
3. Launch a virtual machine using a supported operating system.
4. Configure network access and firewall rules.
5. Install the required tools.
6. Test connectivity and update the system.
7. Shut down unused resources to avoid unnecessary charges.
Useful Linux commands for checking the environment
uname -a
cat /etc/os-release
ip -br addr
ip route
df -h
free -h


Security precautions
- Enable multi-factor authentication on cloud accounts.
- Use strong credentials and least-privilege access.
- Do not expose SSH or other administrative ports unnecessarily.
- Never publish access keys or passwords in GitHub repositories.
- Monitor cloud usage and billing.