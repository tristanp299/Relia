# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/xml/_quick_tcp_nmap.xml 192.168.224.247
Increasing send delay for 192.168.224.247 from 0 to 5 due to 59 out of 146 dropped probes since last increase.
adjust_timeouts2: packet supposedly had rtt of -353888 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -675276 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -675276 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -679744 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -679744 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -679932 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -679932 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -979429 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -979429 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.074s latency).
Scanned at 2024-04-02 20:56:40 PDT for 88s
Not shown: 994 closed tcp ports (reset)
PORT     STATE SERVICE       REASON          VERSION
80/tcp   open  http          syn-ack ttl 125 Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: RELIA - New Hire Information
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
135/tcp  open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
443/tcp  open  ssl/http      syn-ack ttl 125 Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: RELIA - New Hire Information
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
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
| tls-alpn: 
|_  http/1.1
|_ssl-date: TLS randomness does not represent time
445/tcp  open  microsoft-ds? syn-ack ttl 125
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
|_ssl-date: 2024-04-03T03:58:06+00:00; 0s from scanner time.
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
|_  System_Time: 2024-04-03T03:57:56+00:00
Device type: general purpose|firewall
Running (JUST GUESSING): Linux 2.6.X (87%), Fortinet embedded (85%), Microsoft Windows Vista (85%)
OS CPE: cpe:/o:linux:linux_kernel:2.6.28 cpe:/o:microsoft:windows_vista::sp1:home_premium
Aggressive OS guesses: Linux 2.6.28 (87%), Fortinet FortiGate-60B or -100A firewall (85%), Microsoft Windows Vista Home Premium SP1 (85%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=43399%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:3D0%P=aarch64-unknown-linux-gnu)SEQ()SEQ(SP=F6%GCD=1%ISR=103%TS=A)SEQ(SP
OS:=FB%GCD=1%ISR=107%TS=A)OPS(O1=M551NW8ST11%O2=M551NW8ST11%O3=M551NW8NNT11
OS:%O4=M551NW8ST11%O5=M551NW8ST11%O6=M551ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W
OS:4=FFFF%W5=FFFF%W6=FFDC)ECN(R=N)ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC=
OS:Y%Q=)T1(R=N)T1(R=Y%DF=Y%T=80%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)
OS:T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T7(R=N)U1(R=N)U1(R=
OS:Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=4AE7%RUD=G)IE(R=N)

Uptime guess: 0.005 days (since Tue Apr  2 20:51:31 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=246 (Good luck!)
IP ID Sequence Generation: Busy server or unknown class
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| smb2-time: 
|   date: 2024-04-03T03:57:57
|_  start_date: N/A
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 58263/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 10381/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 12958/udp): CLEAN (Timeout)
|   Check 4 (port 36024/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked

TRACEROUTE (using port 587/tcp)
HOP RTT      ADDRESS
1   72.02 ms 192.168.45.1
2   72.00 ms 192.168.45.254
3   73.70 ms 192.168.251.1
4   72.93 ms 192.168.224.247

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:08 2024 -- 1 IP address (1 host up) scanned in 88.73 seconds
