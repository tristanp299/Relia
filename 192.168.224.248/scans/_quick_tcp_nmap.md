# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/xml/_quick_tcp_nmap.xml 192.168.224.248
Increasing send delay for 192.168.224.248 from 0 to 5 due to 90 out of 224 dropped probes since last increase.
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
adjust_timeouts2: packet supposedly had rtt of -353618 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -429595 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -429595 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -428723 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -428723 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -281501 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -281501 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -302790 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -302790 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -954637 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -954637 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 20:56:40 PDT for 85s
Not shown: 995 closed tcp ports (reset)
PORT     STATE SERVICE       REASON          VERSION
80/tcp   open  http          syn-ack ttl 125 Microsoft IIS httpd 10.0
|_http-favicon: Unknown favicon MD5: 2DE6897008EB657D2EC770FE5B909439
|_http-title: Home
| http-robots.txt: 16 disallowed entries 
| /*/ctl/ /admin/ /App_Browsers/ /App_Code/ /App_Data/ 
| /App_GlobalResources/ /bin/ /Components/ /Config/ /contest/ /controls/ 
| /Documentation/ /HttpModules/ /Install/ /Providers/ 
|_/Activity-Feed/userId/
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
135/tcp  open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? syn-ack ttl 125
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| ssl-cert: Subject: commonName=EXTERNAL
| Issuer: commonName=EXTERNAL
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-04-02T03:51:10
| Not valid after:  2024-10-02T03:51:10
| MD5:   a584:bf4a:b48c:d730:436b:18f8:820a:32ee
| SHA-1: 5c85:e2ad:976d:8022:e913:8ab9:d6c4:333e:c6b8:5311
| -----BEGIN CERTIFICATE-----
| MIIC1DCCAbygAwIBAgIQFve+lwKgxrBIfE+bDvTHbDANBgkqhkiG9w0BAQsFADAT
| MREwDwYDVQQDEwhFWFRFUk5BTDAeFw0yNDA0MDIwMzUxMTBaFw0yNDEwMDIwMzUx
| MTBaMBMxETAPBgNVBAMTCEVYVEVSTkFMMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8A
| MIIBCgKCAQEA56oZDQTDXOkiRVHOam3X3cCkYXmnyUzkGgfj3d/ivGFrGXSwqF8R
| Yo6R0GtTDAnA/mDXxPMVIZn6X4R8e+OBjI3l33auLZlulnbVcVV14U7wD7MDdmxi
| vUO/rGLgQiM4S2kqRbV/TFIY8lLkeQm8pyusEK2SR/d6ePd/w5SgHQayqmbtTvB9
| VtdMJyqf47A2WkGfp0DbvfUVvXQokekP6wc9uEjRwvJXYf6qRN1MyrcbZwkROQ+d
| 7YIkIlyDqPF0zlCmlrDtfAxaqJYzQxRAJ1N1SPXwGSd2vFg21kKEhtAdGJnA7B2I
| p2hBv0tM32KGjOCm6lLNgdMQt7VHFu/8ZQIDAQABoyQwIjATBgNVHSUEDDAKBggr
| BgEFBQcDATALBgNVHQ8EBAMCBDAwDQYJKoZIhvcNAQELBQADggEBAFislqelLcB7
| VzIbb+Ch9dEEJIz99tcgpZLw3jT8aEHvLtrH6XAZ1bj3UjWS+RnoXfBOpB7PAYw4
| SQIyeJb0chLBEdS/OsATF7wEMS/oaHM2fCHYcVBH6+ZR+bmeswJMNFBeSPA1TzB4
| xPMZUc7Jq3rLepXmoZRoIzIKAoYZRr7eXpJtpO3U4P6seM3abdRbjdzduE5GjARt
| nqb+qFhLRu9nkxV9EIWTj0qlfNPzTB4Gg9+El/DMcMaEXTJU/gxQ2XKHut6yWSdk
| H4MtV5ENWDn4hGip+g5AoXgy6KF6s10FBkNZPpEdM14c8wjQwJeMMQINxryw6p/r
| Y6br6Wk8ydg=
|_-----END CERTIFICATE-----
| rdp-ntlm-info: 
|   Target_Name: EXTERNAL
|   NetBIOS_Domain_Name: EXTERNAL
|   NetBIOS_Computer_Name: EXTERNAL
|   DNS_Domain_Name: EXTERNAL
|   DNS_Computer_Name: EXTERNAL
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T03:57:56+00:00
|_ssl-date: 2024-04-03T03:58:05+00:00; 0s from scanner time.
Device type: general purpose|broadband router
Running (JUST GUESSING): Microsoft Windows 2022|2019|2012|2016|2008|7 (92%), Linux 3.X|4.X|2.6.X (91%)
OS CPE: cpe:/o:microsoft:windows_server_2012 cpe:/o:microsoft:windows_server_2016 cpe:/o:linux:linux_kernel:3 cpe:/o:linux:linux_kernel:4.0 cpe:/o:linux:linux_kernel:2.6.32 cpe:/o:linux:linux_kernel:2.6.31 cpe:/o:microsoft:windows_server_2008:r2 cpe:/o:microsoft:windows_7::sp1
Aggressive OS guesses: Microsoft Windows Server 2022 (92%), Microsoft Windows Server 2019 (92%), Microsoft Windows Server 2012 (91%), Microsoft Windows Server 2012 or Windows Server 2012 R2 (91%), Microsoft Windows Server 2012 R2 (91%), Microsoft Windows Server 2016 (91%), Linux 3.0 - 3.2 (91%), Linux 4.0 (90%), Linux 2.6.32 (90%), Linux 2.6.31 (89%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=31122%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:3CD%P=aarch64-unknown-linux-gnu)SEQ()SEQ(SP=107%GCD=1%ISR=108%TS=A)SEQ(S
OS:P=107%GCD=4%ISR=108%TI=I%TS=A)SEQ(SP=FC%GCD=2%ISR=101%TI=RD%TS=C)SEQ(SP=
OS:FD%GCD=1%ISR=107%TS=A)OPS(O1=M551NW8ST11%O2=M551NW8ST11%O3=M551NW8NNT11%
OS:O4=M551NW8ST11%O5=M551NW8ST11%O6=M551ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4
OS:=FFFF%W5=FFFF%W6=FFDC)ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC=Y%Q=)T1(R
OS:=Y%DF=Y%T=80%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)T5(R=Y%DF=Y%T=80
OS:%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T7(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=
OS:0%RIPL=G%RID=G%RIPCK=G%RUCK=A7A4%RUD=G)IE(R=N)

Uptime guess: 0.007 days (since Tue Apr  2 20:48:39 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=253 (Good luck!)
IP ID Sequence Generation: Busy server or unknown class
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required
| smb2-time: 
|   date: 2024-04-03T03:57:57
|_  start_date: N/A
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 17086/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 4156/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 45331/udp): CLEAN (Failed to receive data)
|   Check 4 (port 52002/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked

TRACEROUTE (using port 22/tcp)
HOP RTT      ADDRESS
1   72.02 ms 192.168.45.1
2   72.05 ms 192.168.45.254
3   74.20 ms 192.168.251.1
4   73.45 ms 192.168.224.248

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:05 2024 -- 1 IP address (1 host up) scanned in 85.67 seconds
