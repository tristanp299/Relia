# Nmap 7.94SVN scan initiated Tue Apr  2 21:09:00 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 445 "--script=banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp445/tcp_445_smb_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp445/xml/tcp_445_smb_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.097s latency).
Scanned at 2024-04-02 21:09:00 PDT for 75s

PORT    STATE SERVICE       REASON          VERSION
445/tcp open  microsoft-ds? syn-ack ttl 125
|_smb-enum-services: ERROR: Script execution failed (use -d to debug)

Host script results:
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required
| smb2-time: 
|   date: 2024-04-03T04:09:48
|_  start_date: N/A
| smb-protocols: 
|   dialects: 
|     2:0:2
|     2:1:0
|     3:0:0
|     3:0:2
|_    3:1:1
| smb-mbenum: 
|_  ERROR: Failed to connect to browser service: Could not negotiate a connection:SMB: Failed to receive bytes: ERROR
|_smb-print-text: false
|_smb-vuln-ms10-061: Could not negotiate a connection:SMB: Failed to receive bytes: ERROR
| smb2-capabilities: 
|   2:0:2: 
|     Distributed File System
|   2:1:0: 
|     Distributed File System
|     Leasing
|     Multi-credit operations
|   3:0:0: 
|     Distributed File System
|     Leasing
|     Multi-credit operations
|   3:0:2: 
|     Distributed File System
|     Leasing
|     Multi-credit operations
|   3:1:1: 
|     Distributed File System
|     Leasing
|_    Multi-credit operations

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:10:15 2024 -- 1 IP address (1 host up) scanned in 74.65 seconds
