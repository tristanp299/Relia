# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/_full_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/xml/_full_tcp_nmap.xml 192.168.224.248
Increasing send delay for 192.168.224.248 from 0 to 5 due to 64 out of 159 dropped probes since last increase.
Warning: 192.168.224.248 giving up on port because retransmission cap hit (6).
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.11s latency).
Scanned at 2024-04-02 20:56:40 PDT for 282s
Not shown: 65494 closed tcp ports (reset)
PORT      STATE    SERVICE       REASON          VERSION
80/tcp    open     http          syn-ack ttl 125 Microsoft IIS httpd 10.0
| http-robots.txt: 16 disallowed entries 
| /*/ctl/ /admin/ /App_Browsers/ /App_Code/ /App_Data/ 
| /App_GlobalResources/ /bin/ /Components/ /Config/ /contest/ /controls/ 
| /Documentation/ /HttpModules/ /Install/ /Providers/ 
|_/Activity-Feed/userId/
|_http-favicon: Unknown favicon MD5: 2DE6897008EB657D2EC770FE5B909439
|_http-title: Home
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
135/tcp   open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp   open     netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
445/tcp   open     microsoft-ds? syn-ack ttl 125
1512/tcp  filtered wins          no-response
3091/tcp  filtered 1ci-smcs      no-response
3389/tcp  open     ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
|_ssl-date: 2024-04-03T04:01:21+00:00; 0s from scanner time.
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
|_  System_Time: 2024-04-03T04:01:10+00:00
5985/tcp  open     http          syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Not Found
6100/tcp  filtered synchronet-db no-response
6482/tcp  filtered ldoms-mgmt    no-response
9629/tcp  filtered uniport       no-response
9695/tcp  filtered ccnx          no-response
15861/tcp filtered unknown       no-response
16386/tcp filtered unknown       no-response
18799/tcp filtered unknown       no-response
24698/tcp filtered unknown       no-response
27032/tcp filtered unknown       no-response
27257/tcp filtered unknown       no-response
27685/tcp filtered unknown       no-response
28064/tcp filtered unknown       no-response
29318/tcp filtered unknown       no-response
32849/tcp filtered unknown       no-response
37539/tcp filtered unknown       no-response
39347/tcp filtered unknown       no-response
47001/tcp open     http          syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Not Found
|_http-server-header: Microsoft-HTTPAPI/2.0
47268/tcp filtered unknown       no-response
49543/tcp filtered unknown       no-response
49664/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49665/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49666/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49667/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49668/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49669/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49670/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49965/tcp open     ms-sql-s      syn-ack ttl 125 Microsoft SQL Server 2019 15.00.2000.00; RTM
| ms-sql-info: 
|   192.168.224.248:49965: 
|     Version: 
|       name: Microsoft SQL Server 2019 RTM
|       number: 15.00.2000.00
|       Product: Microsoft SQL Server 2019
|       Service pack level: RTM
|       Post-SP patches applied: false
|_    TCP port: 49965
| ssl-cert: Subject: commonName=SSL_Self_Signed_Fallback
| Issuer: commonName=SSL_Self_Signed_Fallback
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2023-03-01T06:42:58
| Not valid after:  2053-03-01T06:42:58
| MD5:   022f:e745:145a:cada:c06e:cb13:239b:465d
| SHA-1: a905:ee65:7daa:11d2:a294:82d2:b3c9:3b94:6d72:9373
| -----BEGIN CERTIFICATE-----
| MIIDADCCAeigAwIBAgIQOtQrLNfn+IhF0ZXlptCaojANBgkqhkiG9w0BAQsFADA7
| MTkwNwYDVQQDHjAAUwBTAEwAXwBTAGUAbABmAF8AUwBpAGcAbgBlAGQAXwBGAGEA
| bABsAGIAYQBjAGswIBcNMjMwMzAxMDY0MjU4WhgPMjA1MzAzMDEwNjQyNThaMDsx
| OTA3BgNVBAMeMABTAFMATABfAFMAZQBsAGYAXwBTAGkAZwBuAGUAZABfAEYAYQBs
| AGwAYgBhAGMAazCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEBAOGZFIF+
| tnPKxnC2Ac0Gtn/pM812NYNpaqxNImrILilpHDIVxklXE7EiO3PLfsB9mtAKeXKh
| 2NpPN0CN4p8Oe1LyozKJuHKpf9B4xgHHrU7WM2h8XU4zGmPvQ4j3ULfh+3jkr1Xm
| hboAUze5IMrUomdtU2224c+aI2vSVJOLKZ2n6iaBbpFVx26wcJp/D5ATKwoHu+fq
| g0UScRl8ElU0qx17zs2HtmQIXSV83wg7IatAturL4cmULjKrtPTzIsImOjtXzKdP
| +Mj7uYP8Akfr9xNazgcBYvivLEn1v60k80vOL49gWa/gmk0/P8A2tHvkWsGRbq0R
| 3+GNAjhdlLUBHt0CAwEAATANBgkqhkiG9w0BAQsFAAOCAQEAVu1e7C+HcvZiN1OV
| eNKcgwU0VLEh4nkKwLHJ8HfdCEZ79YscSVuk042QN0FFVUuNZR9SwiYb9wY+pjvj
| 2NpDrK7UcgYTXZY4nXZLC+pTurcBC24nD3ZE38RGJnXkt9lW1WSbCBX2/QaQHeCT
| dEUoWGy5DAo0f0AwUHK2Q+5diuqjwD1gAgJEy3GsjQOUym99Qc+iP7a4c8qbvLdS
| SY+zgQFfrqmKsZ/LKI7ypPa1uorDneCSH7uhr67mqWgGMfDOn4D9g/U9q3TM7lLN
| tb/yIgCrlIaoAmFep+qbMquxa7kh4M6NnkINsuD/QESDEb0z1lqhB6ZOhDWCq/to
| dtwIrQ==
|_-----END CERTIFICATE-----
| ms-sql-ntlm-info: 
|   192.168.224.248:49965: 
|     Target_Name: EXTERNAL
|     NetBIOS_Domain_Name: EXTERNAL
|     NetBIOS_Computer_Name: EXTERNAL
|     DNS_Domain_Name: EXTERNAL
|     DNS_Computer_Name: EXTERNAL
|_    Product_Version: 10.0.20348
|_ssl-date: 2024-04-03T04:01:21+00:00; 0s from scanner time.
50372/tcp filtered unknown       no-response
50882/tcp filtered unknown       no-response
51786/tcp filtered unknown       no-response
58943/tcp filtered unknown       no-response
60339/tcp filtered unknown       no-response
61320/tcp filtered unknown       no-response
Aggressive OS guesses: Microsoft Windows Server 2008 R2 (88%), Microsoft Windows 7 SP1 (88%), Linux 2.6.30 (88%), Microsoft Windows Server 2008 (88%), Microsoft Windows Server 2008 R2 or Windows 8 (87%), Microsoft Windows Server 2008 R2 SP1 (87%), Microsoft Windows 8.1 R1 (87%), Microsoft Windows 7 or Windows Server 2008 R2 (86%), Microsoft Windows Server 2008 or 2008 Beta 3 (86%), Microsoft Windows Server 2008 SP1 or Windows Server 2008 R2 (86%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=32187%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:492%P=aarch64-unknown-linux-gnu)SEQ()SEQ(TI=RD%TS=F)ECN(R=N)ECN(R=Y%DF=Y
OS:%T=80%W=1FFE%O=NNT11%CC=N%Q=)ECN(R=Y%DF=Y%T=80%W=1FFF%O=NNT11%CC=N%Q=)EC
OS:N(R=Y%DF=Y%T=80%W=2000%O=NNT11%CC=N%Q=)T1(R=N)T1(R=Y%DF=Y%T=80%S=O%A=O%F
OS:=AS%RD=0%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T2(R=Y%DF=Y%T=
OS:80%W=1FFD%S=O%A=O%F=A%O=NNT11%RD=0%Q=)T2(R=Y%DF=Y%T=80%W=2000%S=O%A=O%F=
OS:A%O=NNT11%RD=0%Q=)T2(R=Y%DF=Y%T=80%W=2001%S=O%A=O%F=A%O=NNT11%RD=0%Q=)T3
OS:(R=N)T4(R=N)T4(R=Y%DF=Y%T=80%W=1FFF%S=O%A=O%F=A%O=NNT11%RD=0%Q=)T5(R=N)T
OS:5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T6(R=Y%DF=Y%T=80%W=2
OS:001%S=O%A=O%F=A%O=NNT11%RD=0%Q=)T7(R=N)U1(R=N)U1(R=Y%DF=N%T=80%IPL=164%U
OS:N=0%RIPL=G%RID=G%RIPCK=G%RUCK=A168%RUD=G)IE(R=N)

Uptime guess: 0.000 days (since Tue Apr  2 21:00:39 2024)
Network Distance: 4 hops
IP ID Sequence Generation: Randomized
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-time: 
|   date: 2024-04-03T04:01:14
|_  start_date: N/A
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 17086/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 4156/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 45331/udp): CLEAN (Failed to receive data)
|   Check 4 (port 52002/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE (using port 587/tcp)
HOP RTT      ADDRESS
1   73.36 ms 192.168.45.1
2   73.26 ms 192.168.45.254
3   75.79 ms 192.168.251.1
4   75.85 ms 192.168.224.248

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:01:22 2024 -- 1 IP address (1 host up) scanned in 282.79 seconds
