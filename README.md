
CYBERSECURITY iNTERNSHIP - ELEVATE LABS --------------REPORT FILE -------------- 
TASK 1 :- SCAN LOCAL NETWORK FOR OPEN PORTS OBJECTIVE :- Discover open ports on devices in your local network . 
-----------TOOLS FOR SCANNING ---------- 
Nmap :- Nmap, short for Network Mapper, is an open-source network scanning tool used for network discovery and security auditing. 
or
wireshark:- Wireshark is a network packet analyzer that captures and examines data packets traveling through a network. 
-----------PROCEDURE---------- 
STEP1: Go To CMD and RUN command "ipconfig" to identify your local ip range . Output:- IP 192.168.101.1 
subnet mask :- 255.255.255.0 
which is belong from Class A

Step2:-Download and Install Nmap in your device 
step3:- Run command nmap -sS 192.168.101.1 Results:- Starting Nmap 7.95 ( https://nmap.org ) at 2025-08-04 08:37 EDT Nmap scan report for 192.168.101.1 Host is up (0.0012s latency). Not shown: 995 filtered tcp ports (no-response) PORT STATE SERVICE 135/tcp open msrpc 139/tcp open netbios-ssn 445/tcp open microsoft-ds 902/tcp open iss-realsecure 912/tcp open apex-mesh

Nmap done: 1 IP address (1 host up) scanned in 4.81 seconds

CYBERSECURITY INTERNSHIP - ELEVATE LABS
REPORT FILE: 
TASK 1 - Scan Local Network for Open Ports
📌 Objective
The main objective of this task is to discover open ports on devices in the local network for network security analysis.

🛠 Tools Used for Scanning
1. Nmap (Network Mapper)
Purpose: Open-source network scanning tool used for network discovery and security auditing.

Official Website: https://nmap.org

2. Wireshark 
Purpose: Network packet analyzer that captures and examines data packets traveling through a network.

Official Website: https://www.wireshark.org

⚙️ Procedure
Step 1: Identify Local IP Range
Open Command Prompt (CMD)

Run the command:

ipconfig
Example Output:

IPv4 Address    : 192.168.101.1
Subnet Mask     : 255.255.255.0
This shows the device is in the Class A IP range.

Step 2: Install Nmap
Download and install Nmap from https://nmap.org/download.html

Step 3: Scan the Local Network for Open Ports
Open terminal or CMD and run:

nmap -sS 192.168.101.1
Sample Output:

Starting Nmap 7.95 ( https://nmap.org ) at 2025-08-04 08:37 EDT
Nmap scan report for 192.168.101.1
Host is up (0.0012s latency).
Not shown: 995 filtered tcp ports (no-response)
PORT     STATE SERVICE
135/tcp  open  msrpc
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
902/tcp  open  iss-realsecure
912/tcp  open  apex-mesh

Nmap done: 1 IP address (1 host up) scanned in 4.81 seconds
📊 Results and Analysis
Open Ports Detected: 135, 139, 445, 902, 912

Implication:

Ports 135, 139, and 445 are commonly used for Windows Networking (SMB) and may be vulnerable to attacks if not secured.

Ports 902 and 912 may indicate VMware or other services running.

✅ Conclusion
Successfully scanned the local network for open ports.

Discovered 5 open ports on the target device.

This analysis can be used for network hardening and security auditing.
<img width="647" height="270" alt="result ss" src="https://github.com/user-attachments/assets/facbca83-0548-44b1-a365-5717721b44cc" />

