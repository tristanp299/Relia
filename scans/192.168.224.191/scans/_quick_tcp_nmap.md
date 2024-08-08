# Nmap 7.94SVN scan initiated Tue Apr  2 21:01:03 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.191/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.191/scans/xml/_quick_tcp_nmap.xml 192.168.224.191
adjust_timeouts2: packet supposedly had rtt of -756053 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -756053 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -380401 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -380401 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -673845 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -673845 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -680652 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -680652 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -605754 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -605754 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.191
Host is up, received user-set (0.083s latency).
Scanned at 2024-04-02 21:01:04 PDT for 101s
Not shown: 995 closed tcp ports (reset)
PORT     STATE SERVICE       REASON          VERSION
80/tcp   open  http          syn-ack ttl 125 Microsoft IIS httpd 10.0
|_http-server-header: Microsoft-IIS/10.0
| http-auth: 
| HTTP/1.1 401 Unauthorized\x0D
|_  Basic realm=192.168.224.191
|_http-title: 401 - Unauthorized: Access is denied due to invalid credentials.
135/tcp  open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? syn-ack ttl 125
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| ssl-cert: Subject: commonName=login.relia.com
| Issuer: commonName=login.relia.com
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-04-02T03:51:24
| Not valid after:  2024-10-02T03:51:24
| MD5:   a11e:74d0:3e26:9798:2cd2:23b4:042e:7ea8
| SHA-1: 7baa:db80:8004:6091:c748:8c30:31ec:b549:df13:cbc4
| -----BEGIN CERTIFICATE-----
| MIIC4jCCAcqgAwIBAgIQdtruqDnQ7o1IYp27loS04zANBgkqhkiG9w0BAQsFADAa
| MRgwFgYDVQQDEw9sb2dpbi5yZWxpYS5jb20wHhcNMjQwNDAyMDM1MTI0WhcNMjQx
| MDAyMDM1MTI0WjAaMRgwFgYDVQQDEw9sb2dpbi5yZWxpYS5jb20wggEiMA0GCSqG
| SIb3DQEBAQUAA4IBDwAwggEKAoIBAQC8DfO9QNR6IxkrhxgIcZJlF9X079dzXb6N
| Q8qp64tpPKS27rkJXJPbkqNL+46rx10B9pZZ+WH0bo6AEzxfOmlckq9Fe6cyhC6m
| vhJcO4z58Rw9zf80K9LgSDLIE6+QplWGyTMuI9kSAyfLWlUxse16YCuDqlg+H+LT
| XHrGkBPsuIrsl+MRWcGJzl7DhhAVCuoN+MW9TgEGbzyos8Sk+KrmnSADFmZB4cy6
| QfhQJQ6NpZGrc6piG/88fLikkfHg39xjxulOStJBiTqAkTjTonrCmTaCkPKn/m3d
| 5bSkGasE85nDV7VK0DHBdVyVPNbnJzbseEGNEEWj71yW6EigR5/9AgMBAAGjJDAi
| MBMGA1UdJQQMMAoGCCsGAQUFBwMBMAsGA1UdDwQEAwIEMDANBgkqhkiG9w0BAQsF
| AAOCAQEACXRXVXR8GGwZfbEoeWtaYarPb3tckZSBigGZQPztq86zO4qZELPiKxsp
| s0YCWsbkoQxS9FrZNhHPgGTeMRbhVPo2X88imYAiRArPl8MRMuVnerfgrMl95J+I
| j4wWtE2MquG6YiReFaHnQXaOxn6x4ePSWz8qooQ6+Yv3yzFgo4uKTdiTeYzNrP66
| 1BeeUNlgmnOuB6jkA4uTz94wvL56W+gQho+Y7Y4xPHkfZ7ec/Q7jBiNgquC/2PEN
| zcOLE6hcvFvV3L+RvvuNsslXmdXUSDW8YUx1F7s1id1jBFPqLnXC/fpK9BkG8Nr1
| Al1W/WvjrrFH0KMIayCzSTLjzPBxNw==
|_-----END CERTIFICATE-----
|_ssl-date: 2024-04-03T04:02:44+00:00; 0s from scanner time.
| rdp-ntlm-info: 
|   Target_Name: RELIA
|   NetBIOS_Domain_Name: RELIA
|   NetBIOS_Computer_Name: LOGIN
|   DNS_Domain_Name: relia.com
|   DNS_Computer_Name: login.relia.com
|   DNS_Tree_Name: relia.com
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T04:02:34+00:00
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows 2022 (88%)
Aggressive OS guesses: Microsoft Windows Server 2022 (88%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=34962%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:4E5%P=aarch64-unknown-linux-gnu)SEQ(SP=101%GCD=1%ISR=10B%TS=A)SEQ(SP=102
OS:%GCD=1%ISR=10B%TS=A)SEQ(SP=102%GCD=1%ISR=10C%TS=A)OPS(O1=M551NW8ST11%O2=
OS:M551NW8ST11%O3=M551NW8NNT11%O4=M551NW8ST11%O5=M551NW8ST11%O6=M551ST11)WI
OS:N(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FFDC)ECN(R=Y%DF=Y%T=80%W=FF
OS:FF%O=M551NW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3
OS:(R=N)T4(R=N)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T7(R=N)
OS:U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=64BE%RUD=G)IE(R=
OS:N)

Uptime guess: 0.010 days (since Tue Apr  2 20:48:30 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=258 (Good luck!)
IP ID Sequence Generation: Busy server or unknown class
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 30372/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 47919/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 6821/udp): CLEAN (Timeout)
|   Check 4 (port 57822/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
| smb2-time: 
|   date: 2024-04-03T04:02:38
|_  start_date: N/A
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE (using port 23/tcp)
HOP RTT      ADDRESS
1   72.62 ms 192.168.45.1
2   72.56 ms 192.168.45.254
3   ...
4   92.47 ms 192.168.224.191

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:02:45 2024 -- 1 IP address (1 host up) scanned in 101.77 seconds
