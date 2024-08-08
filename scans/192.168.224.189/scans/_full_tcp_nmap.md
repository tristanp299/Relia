# Nmap 7.94SVN scan initiated Tue Apr  2 21:02:45 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/_full_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/xml/_full_tcp_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 21:02:45 PDT for 282s
Not shown: 65519 closed tcp ports (reset)
PORT      STATE SERVICE       REASON          VERSION
25/tcp    open  smtp          syn-ack ttl 125 hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
110/tcp   open  pop3          syn-ack ttl 125 hMailServer pop3d
|_pop3-capabilities: TOP UIDL USER
135/tcp   open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp   open  netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
143/tcp   open  imap          syn-ack ttl 125 hMailServer imapd
|_imap-capabilities: RIGHTS=texkA0001 completed CAPABILITY ACL IDLE QUOTA IMAP4rev1 OK CHILDREN NAMESPACE SORT IMAP4
445/tcp   open  microsoft-ds? syn-ack ttl 125
587/tcp   open  smtp          syn-ack ttl 125 hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
5985/tcp  open  http          syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
47001/tcp open  http          syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
49664/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
49665/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
49666/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
49667/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
49668/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
49669/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
49670/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows 2022 (89%)
Aggressive OS guesses: Microsoft Windows Server 2022 (89%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=25%CT=1%CU=36849%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:5FF%P=aarch64-unknown-linux-gnu)SEQ(SP=105%GCD=1%ISR=107%TI=RD%TS=B)SEQ(
OS:SP=105%GCD=1%ISR=107%TI=RD%TS=C)OPS(O1=M551NW8ST11%O2=M551NW8ST11%O3=M55
OS:1NW8NNT11%O4=M551NW8ST11%O5=M551NW8ST11%O6=M551ST11)WIN(W1=FFFF%W2=FFFF%
OS:W3=FFFF%W4=FFFF%W5=FFFF%W6=FFDC)ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC
OS:=N%Q=)ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O
OS:%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=
OS:AR%O=%RD=0%Q=)T6(R=N)T7(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%R
OS:IPCK=G%RUCK=990D%RUD=G)IE(R=N)

Uptime guess: 0.005 days (since Tue Apr  2 20:59:56 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=261 (Good luck!)
IP ID Sequence Generation: Randomized
Service Info: Host: MAIL; OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-time: 
|   date: 2024-04-03T04:07:13
|_  start_date: N/A
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 18226/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 54478/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 36637/udp): CLEAN (Failed to receive data)
|   Check 4 (port 28753/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required
|_clock-skew: 0s

TRACEROUTE (using port 8888/tcp)
HOP RTT      ADDRESS
1   73.49 ms 192.168.45.1
2   73.47 ms 192.168.45.254
3   ...
4   80.08 ms 192.168.224.189

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:07:27 2024 -- 1 IP address (1 host up) scanned in 282.38 seconds
