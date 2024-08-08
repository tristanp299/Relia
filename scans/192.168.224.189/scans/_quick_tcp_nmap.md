# Nmap 7.94SVN scan initiated Tue Apr  2 21:02:18 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/xml/_quick_tcp_nmap.xml 192.168.224.189
adjust_timeouts2: packet supposedly had rtt of -577379 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -577379 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -553407 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -553407 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -563584 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -563584 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -569390 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -569390 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -298666 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -298666 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -325922 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -325922 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -428424 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -428424 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -187577 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -187577 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -196163 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -196163 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -202614 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -202614 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -201593 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -201593 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -264824 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -264824 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.082s latency).
Scanned at 2024-04-02 21:02:18 PDT for 110s
Not shown: 993 closed tcp ports (reset)
PORT    STATE SERVICE       REASON          VERSION
25/tcp  open  smtp          syn-ack ttl 125 hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
110/tcp open  pop3          syn-ack ttl 125 hMailServer pop3d
|_pop3-capabilities: USER UIDL TOP
135/tcp open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp open  netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
143/tcp open  imap          syn-ack ttl 125 hMailServer imapd
|_imap-capabilities: NAMESPACE QUOTA CAPABILITY IMAP4rev1 CHILDREN OK ACL IDLE completed RIGHTS=texkA0001 IMAP4 SORT
445/tcp open  microsoft-ds? syn-ack ttl 125
587/tcp open  smtp          syn-ack ttl 125 hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows 2022 (89%)
Aggressive OS guesses: Microsoft Windows Server 2022 (89%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=25%CT=1%CU=42078%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:538%P=aarch64-unknown-linux-gnu)SEQ(TI=RD%TS=D)SEQ(SP=104%GCD=1%ISR=10B%
OS:TI=RD%TS=C)SEQ(SP=104%GCD=2%ISR=10B%TS=A)SEQ(SP=105%GCD=2%ISR=10C%TI=RD%
OS:TS=C)OPS(O1=M551NW8ST11%O2=M551NW8ST11%O3=M551NW8NNT11%O4=M551NW8ST11%O5
OS:=M551NW8ST11%O6=M551ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=
OS:FFDC)ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O%
OS:A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=A
OS:R%O=%RD=0%Q=)T6(R=N)T7(R=N)U1(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%R
OS:ID=G%RIPCK=G%RUCK=5496%RUD=G)IE(R=N)

Uptime guess: 0.003 days (since Tue Apr  2 21:00:26 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=260 (Good luck!)
IP ID Sequence Generation: Randomized
Service Info: Host: MAIL; OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 18226/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 54478/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 36637/udp): CLEAN (Timeout)
|   Check 4 (port 28753/udp): CLEAN (Failed to receive data)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
|_clock-skew: 0s
| smb2-time: 
|   date: 2024-04-03T04:03:59
|_  start_date: N/A
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE (using port 993/tcp)
HOP RTT      ADDRESS
1   74.07 ms 192.168.45.1
2   74.05 ms 192.168.45.254
3   ...
4   83.65 ms 192.168.224.189

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:04:08 2024 -- 1 IP address (1 host up) scanned in 110.77 seconds
