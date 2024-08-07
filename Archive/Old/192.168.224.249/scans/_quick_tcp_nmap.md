# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.249/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.249/scans/xml/_quick_tcp_nmap.xml 192.168.224.249
Increasing send delay for 192.168.224.249 from 0 to 5 due to 71 out of 177 dropped probes since last increase.
adjust_timeouts2: packet supposedly had rtt of -351771 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -678311 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -678311 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -428912 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -428912 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -140276 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -140276 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -252988 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -252988 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -1604377 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -1604377 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.249
Host is up, received user-set (0.074s latency).
Scanned at 2024-04-02 20:56:40 PDT for 87s
Not shown: 994 closed tcp ports (reset)
PORT     STATE SERVICE       REASON          VERSION
80/tcp   open  http          syn-ack ttl 125 Microsoft IIS httpd 10.0
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
|_http-server-header: Microsoft-IIS/10.0
|_http-title: IIS Windows Server
135/tcp  open  msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? syn-ack ttl 125
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| rdp-ntlm-info: 
|   Target_Name: LEGACY
|   NetBIOS_Domain_Name: LEGACY
|   NetBIOS_Computer_Name: LEGACY
|   DNS_Domain_Name: LEGACY
|   DNS_Computer_Name: LEGACY
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T03:57:57+00:00
| ssl-cert: Subject: commonName=LEGACY
| Issuer: commonName=LEGACY
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-01-13T23:01:30
| Not valid after:  2024-07-14T23:01:30
| MD5:   ced0:46fb:0382:2c78:4f8e:6e99:7ce2:feaa
| SHA-1: 5931:bfe6:185b:7084:5964:45fb:b55a:3383:85b3:9f7f
| -----BEGIN CERTIFICATE-----
| MIIC0DCCAbigAwIBAgIQYUbza/e+y6VDeQQningixDANBgkqhkiG9w0BAQsFADAR
| MQ8wDQYDVQQDEwZMRUdBQ1kwHhcNMjQwMTEzMjMwMTMwWhcNMjQwNzE0MjMwMTMw
| WjARMQ8wDQYDVQQDEwZMRUdBQ1kwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEK
| AoIBAQCqwka8tAMwtxNQW84u3c2UTguRuAqMNN/4StHyBwGRYKaMS+TfJC/HaWqN
| F0szmrm0L2wTibd/Ndj29TZV0jVOfkTroDoriaHlpjo+cFA6t46e6p0gzuW0K0NK
| 8Npn7FgtlVNgtV8NUvqYq0Juu+z0EhscYh7GhuCdcDLZ1tK6/ehBQkFW96JWpaWo
| Hwus91+dtveOUGxU5+V1UpvW3OkboxoK6Z3bKiqdnevSi5O79BFl9KOQsPJlgwNW
| k8tkWrpAWiSldsNgQ1ZHbKETPdQLFKLPmD0mb8ycw5OIxsaKTwdVbFu/g70UlN5W
| CsMuUJnTiFGpOSHljGDAa7PhN6NVAgMBAAGjJDAiMBMGA1UdJQQMMAoGCCsGAQUF
| BwMBMAsGA1UdDwQEAwIEMDANBgkqhkiG9w0BAQsFAAOCAQEAaUqBAi7tO/D2ZVTy
| N9zEVSnrKvZQ3mJSQNd7Tykw9q4vuMYqmziwd1zrkALTxmWOJ70YTaR14DxQFZ/0
| 9+9TY8d3aeAcA+JxMeSDbXcE2FNCKV8CBc/iD5dUIr+wF3Psb6Va1l3636Al1g9x
| NUMtGoJhfnuxERQOyR+HioGz8dtnK+GSaSfa+4r7jYUySuIL405Cgk0PDPs29D3F
| BrTvzgZsYu8L4tZMOhD8LMMEFQ7axISAUNBRXnAI5/kOkdoCe5m/KMpzIsFi5Pyj
| MPNRNYsGnI+RGBgUpPgtVDGWIvRRkzZ+Ogqw3CUaR9NaxrOLtPMvNjrgUGpd9RR5
| VvEnKg==
|_-----END CERTIFICATE-----
|_ssl-date: 2024-04-03T03:58:07+00:00; 0s from scanner time.
8000/tcp open  http          syn-ack ttl 125 Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/7.4.30)
|_http-open-proxy: Proxy might be redirecting requests
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/7.4.30
| http-title: Welcome to XAMPP
|_Requested resource was http://192.168.224.249:8000/dashboard/
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
Device type: general purpose|broadband router
Running (JUST GUESSING): Microsoft Windows 2022|2019|2012|2016|2008|7 (92%), Linux 3.X|4.X|2.6.X (91%)
OS CPE: cpe:/o:microsoft:windows_server_2012 cpe:/o:microsoft:windows_server_2016 cpe:/o:linux:linux_kernel:3 cpe:/o:linux:linux_kernel:4.0 cpe:/o:linux:linux_kernel:2.6.32 cpe:/o:linux:linux_kernel:2.6.31 cpe:/o:microsoft:windows_server_2008:r2 cpe:/o:microsoft:windows_7::sp1
Aggressive OS guesses: Microsoft Windows Server 2022 (92%), Microsoft Windows Server 2019 (92%), Microsoft Windows Server 2012 (91%), Microsoft Windows Server 2012 or Windows Server 2012 R2 (91%), Microsoft Windows Server 2012 R2 (91%), Microsoft Windows Server 2016 (91%), Linux 3.0 - 3.2 (91%), Linux 4.0 (90%), Linux 2.6.32 (90%), Linux 2.6.31 (89%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=31650%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:3CF%P=aarch64-unknown-linux-gnu)SEQ()SEQ(SP=103%GCD=1%ISR=10E%TS=A)SEQ(S
OS:P=103%GCD=1%ISR=10E%TI=RD%TS=C)SEQ(SP=105%GCD=1%ISR=109%TS=A)OPS(O1=M551
OS:NW8ST11%O2=M551NW8ST11%O3=M551NW8NNT11%O4=M551NW8ST11%O5=M551NW8ST11%O6=
OS:M551ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FFDC)ECN(R=Y%DF=
OS:Y%T=80%W=FFFF%O=M551NW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+%F=AS%RD=0%Q
OS:=)T2(R=N)T3(R=N)T4(R=N)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(
OS:R=N)T7(R=N)U1(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUC
OS:K=5CA6%RUD=G)IE(R=N)

Uptime guess: 0.007 days (since Tue Apr  2 20:48:40 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=261 (Good luck!)
IP ID Sequence Generation: Busy server or unknown class
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 62732/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 51162/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 54655/udp): CLEAN (Timeout)
|   Check 4 (port 8612/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| smb2-time: 
|   date: 2024-04-03T03:57:58
|_  start_date: N/A

TRACEROUTE (using port 110/tcp)
HOP RTT      ADDRESS
1   71.98 ms 192.168.45.1
2   71.95 ms 192.168.45.254
3   74.90 ms 192.168.251.1
4   75.31 ms 192.168.224.249

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:07 2024 -- 1 IP address (1 host up) scanned in 87.69 seconds
