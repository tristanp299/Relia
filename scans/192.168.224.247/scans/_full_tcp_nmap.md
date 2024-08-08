# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/_full_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/xml/_full_tcp_nmap.xml 192.168.224.247
Increasing send delay for 192.168.224.247 from 0 to 5 due to 94 out of 234 dropped probes since last increase.
Warning: 192.168.224.247 giving up on port because retransmission cap hit (6).
adjust_timeouts2: packet supposedly had rtt of -823503 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -823503 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -811933 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -811933 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -815939 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -815939 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -811586 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -811586 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -250715 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -250715 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -216443 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -216443 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -769205 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -769205 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.080s latency).
Scanned at 2024-04-02 20:56:40 PDT for 336s
Not shown: 65499 closed tcp ports (reset)
PORT      STATE    SERVICE         REASON          VERSION
80/tcp    open     http            syn-ack ttl 125 Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-title: RELIA - New Hire Information
| http-methods: 
|_  Supported Methods: POST
135/tcp   open     msrpc           syn-ack ttl 125 Microsoft Windows RPC
139/tcp   open     netbios-ssn     syn-ack ttl 125 Microsoft Windows netbios-ssn
443/tcp   open     tcpwrapped      syn-ack ttl 125
|_http-title: 400 Bad Request
| ssl-cert: Subject: commonName=localhost
| Issuer: commonName=localhost
| Public Key type: rsa
| Public Key bits: 1024
| Signature Algorithm: sha1WithRSAEncryption
| Not valid before: 2009-11-10T23:48:47
| Not valid after:  2019-11-08T23:48:47
| MD5:   a0a4:4cc9:9e84:b26f:9e63:9f9e:d229:dee0
| SHA-1: b023:8c54:7a90:5bfa:119c:4e8b:acca:eacf:3649:1ff6
| -----BEGIN CERTIFICATE-----
| MIIBnzCCAQgCCQC1x1LJh4G1AzANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDEwls
| b2NhbGhvc3QwHhcNMDkxMTEwMjM0ODQ3WhcNMTkxMTA4MjM0ODQ3WjAUMRIwEAYD
| VQQDEwlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBAMEl0yfj
| 7K0Ng2pt51+adRAj4pCdoGOVjx1BmljVnGOMW3OGkHnMw9ajibh1vB6UfHxu463o
| J1wLxgxq+Q8y/rPEehAjBCspKNSq+bMvZhD4p8HNYMRrKFfjZzv3ns1IItw46kgT
| gDpAl1cMRzVGPXFimu5TnWMOZ3ooyaQ0/xntAgMBAAEwDQYJKoZIhvcNAQEFBQAD
| gYEAavHzSWz5umhfb/MnBMa5DL2VNzS+9whmmpsDGEG+uR0kM1W2GQIdVHHJTyFd
| aHXzgVJBQcWTwhp84nvHSiQTDBSaT6cQNQpvag/TaED/SEQpm0VqDFwpfFYuufBL
| vVNbLkKxbK2XwUvu0RxoLdBMC/89HqrZ0ppiONuQ+X2MtxE=
|_-----END CERTIFICATE-----
445/tcp   open     microsoft-ds?   syn-ack ttl 125
1004/tcp  filtered unknown         no-response
3389/tcp  open     ms-wbt-server   syn-ack ttl 125 Microsoft Terminal Services
|_ssl-date: 2024-04-03T04:02:01+00:00; 0s from scanner time.
| ssl-cert: Subject: commonName=WEB02
| Issuer: commonName=WEB02
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-04-02T03:51:09
| Not valid after:  2024-10-02T03:51:09
| MD5:   f22b:9bf1:9594:98da:b395:098d:f202:d2cf
| SHA-1: 832f:3545:10e1:9ae2:9511:7e8c:70ba:bf11:931e:0440
| -----BEGIN CERTIFICATE-----
| MIICzjCCAbagAwIBAgIQMBzqK4I/dYZGHyAZ1HsbEDANBgkqhkiG9w0BAQsFADAQ
| MQ4wDAYDVQQDEwVXRUIwMjAeFw0yNDA0MDIwMzUxMDlaFw0yNDEwMDIwMzUxMDla
| MBAxDjAMBgNVBAMTBVdFQjAyMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKC
| AQEAp01R4pjmdmISv24hs9qEOM2/O3Sz6H7b2xSU7CiCOVnzwc7hJaP5raJFd0am
| 18xDRiOlB4Qks6+snvVeDj/j/gLZh4G4bwfD2G8Wp5lEkwkCQ0qQeMnPaVZxcKM6
| 8BUrYYPwyjFTczXWE2d/7Prinx7xUsjbZrPy7SqqSxXtIeWoUxAuW+vw6dF/TEPZ
| ZM4sOD170dolr5bOcRCEtRDMYUeZSVAHZBTwL5RBuh6qPyEdLhRWS5tLTn374KUS
| Ydse3J7+OrItNpwbBj44ziYmSbPwahfZbhwxWvGGIKbb3KOsrFyvPjT11bk6klz8
| KlT+5ab1Sloc0xCiDiHiMCT8zQIDAQABoyQwIjATBgNVHSUEDDAKBggrBgEFBQcD
| ATALBgNVHQ8EBAMCBDAwDQYJKoZIhvcNAQELBQADggEBAGm9FpqKXZDsW5m2iG5w
| 6sgDJhlv6GSuke7Y6QkiOWajoYxkXUNeCW2l/mzeLE8r5ZIiyKRAD/fWKVWT0dE8
| xd26juMctbXQNhQZ3rTan/p9JylF0crpij70NsapWS8EKUwiYShT0MWXP49ghOPz
| hHvzLCCgHkpLCAgH/AfWe7U8hbscivpgoPT8czyz6LpuB+jXxezvMa+/qEiUs7od
| 5rDivHnA2uNvflShfardw92SIFi+/0Cd8D9wPunM2AvhDuM8H0XrwKcXBjGtCJdg
| rGwHwexpRgwr4y5mzujqI/OupEiU8wMMYxxMS7IFPz+C5XNWWjhyvN+LRtmM2Jvh
| BOQ=
|_-----END CERTIFICATE-----
| rdp-ntlm-info: 
|   Target_Name: WEB02
|   NetBIOS_Domain_Name: WEB02
|   NetBIOS_Computer_Name: WEB02
|   DNS_Domain_Name: WEB02
|   DNS_Computer_Name: WEB02
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T04:00:33+00:00
5985/tcp  open     http            syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-title: Not Found
6078/tcp  filtered unknown         no-response
6274/tcp  filtered unknown         no-response
7235/tcp  filtered aspcoordination no-response
8563/tcp  filtered unknown         no-response
11685/tcp filtered unknown         no-response
14020/tcp open     ftp             syn-ack ttl 125 FileZilla ftpd
|_ftp-bounce: bounce working!
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
|_-r--r--r-- 1 ftp ftp         237639 Nov 04  2022 umbraco.pdf
| ftp-syst: 
|_  SYST: UNIX emulated by FileZilla
14080/tcp open     unknown         syn-ack ttl 125
16547/tcp filtered unknown         no-response
16889/tcp filtered unknown         no-response
17452/tcp filtered unknown         no-response
23143/tcp filtered unknown         no-response
23328/tcp filtered unknown         no-response
24111/tcp filtered unknown         no-response
28571/tcp filtered unknown         no-response
30145/tcp filtered unknown         no-response
37869/tcp filtered unknown         no-response
40042/tcp filtered unknown         no-response
44468/tcp filtered unknown         no-response
47001/tcp open     http            syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-title: Not Found
49664/tcp open     unknown         syn-ack ttl 125
49665/tcp filtered unknown         no-response
49666/tcp open     unknown         syn-ack ttl 125
49667/tcp open     unknown         syn-ack ttl 125
49668/tcp open     unknown         syn-ack ttl 125
49670/tcp open     unknown         syn-ack ttl 125
49671/tcp open     unknown         syn-ack ttl 125
52690/tcp filtered unknown         no-response
53943/tcp filtered unknown         no-response
Device type: general purpose|WAP
Running (JUST GUESSING): Microsoft Windows 2022|2016|10|2019|11 (92%), Linux 2.6.X|3.X|4.X (87%), Aerohive HiveOS 6.X (86%), Minix 2.X (85%)
OS CPE: cpe:/o:microsoft:windows_server_2016 cpe:/o:linux:linux_kernel:2.6.32 cpe:/o:linux:linux_kernel:3.18 cpe:/o:microsoft:windows_10:1607 cpe:/o:aerohive:hiveos:6.8 cpe:/o:minix:minix:2.0.4 cpe:/o:linux:linux_kernel:4.0
Aggressive OS guesses: Microsoft Windows Server 2022 (92%), Microsoft Windows Server 2016 (91%), Linux 2.6.32 (87%), Linux 3.18 (87%), Microsoft Windows 10 1607 (86%), Aerohive HiveOS 6.8 (86%), Linux 2.6.36 (86%), Microsoft Windows Server 2019 (86%), Microsoft Windows 11 21H2 (86%), Minix 2.0.4 (85%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=40339%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:4C8%P=aarch64-unknown-linux-gnu)SEQ(TS=A)SEQ(TI=I%TS=A)SEQ(SP=FC%GCD=1%I
OS:SR=100%TS=A)OPS(O1=M551NW8ST11%O2=M551NW8ST11%O3=M551NW8NNT11%O4=M551NW8
OS:ST11%O5=M551NW8ST11%O6=M551ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=F
OS:FFF%W6=FFDC)ECN(R=N)ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC=Y%Q=)T1(R=Y
OS:%DF=Y%T=80%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)T5(R=N)T5(R=Y%DF=Y
OS:%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T7(R=N)U1(R=N)U1(R=Y%DF=N%T=80
OS:%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=AABE%RUD=G)IE(R=N)

Uptime guess: 0.007 days (since Tue Apr  2 20:51:32 2024)
Network Distance: 4 hops
IP ID Sequence Generation: Incrementing by 2
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 58263/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 10381/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 12958/udp): CLEAN (Timeout)
|   Check 4 (port 36024/udp): CLEAN (Failed to receive data)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
| smb2-time: 
|   date: 2024-04-03T04:00:34
|_  start_date: N/A
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE (using port 1720/tcp)
HOP RTT      ADDRESS
1   83.76 ms 192.168.45.1
2   83.76 ms 192.168.45.254
3   ...
4   77.35 ms 192.168.224.247

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:02:16 2024 -- 1 IP address (1 host up) scanned in 336.37 seconds
