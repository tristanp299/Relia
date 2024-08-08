# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN /home/kali/Documents/Relia/results/192.168.224.249/scans/_full_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.249/scans/xml/_full_tcp_nmap.xml 192.168.224.249
Increasing send delay for 192.168.224.249 from 0 to 5 due to 72 out of 179 dropped probes since last increase.
Warning: 192.168.224.249 giving up on port because retransmission cap hit (6).
Nmap scan report for 192.168.224.249
Host is up, received user-set (0.099s latency).
Scanned at 2024-04-02 20:56:40 PDT for 264s
Not shown: 65500 closed tcp ports (reset)
PORT      STATE    SERVICE       REASON          VERSION
80/tcp    open     http          syn-ack ttl 125 Microsoft IIS httpd 10.0
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
|_http-server-header: Microsoft-IIS/10.0
|_http-title: IIS Windows Server
135/tcp   open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
139/tcp   open     netbios-ssn   syn-ack ttl 125 Microsoft Windows netbios-ssn
445/tcp   open     microsoft-ds? syn-ack ttl 125
1168/tcp  filtered vchat         no-response
2169/tcp  filtered brain         no-response
3389/tcp  open     ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| rdp-ntlm-info: 
|   Target_Name: LEGACY
|   NetBIOS_Domain_Name: LEGACY
|   NetBIOS_Computer_Name: LEGACY
|   DNS_Domain_Name: LEGACY
|   DNS_Computer_Name: LEGACY
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T04:00:55+00:00
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
|_ssl-date: 2024-04-03T04:01:03+00:00; -1s from scanner time.
5280/tcp  filtered xmpp-bosh     no-response
5985/tcp  open     http          syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
7215/tcp  filtered PS-Server     no-response
8000/tcp  open     http          syn-ack ttl 125 Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/7.4.30)
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
| http-title: Welcome to XAMPP
|_Requested resource was http://192.168.224.249:8000/dashboard/
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/7.4.30
|_http-open-proxy: Proxy might be redirecting requests
10779/tcp filtered unknown       no-response
13382/tcp filtered unknown       no-response
15167/tcp filtered unknown       no-response
19065/tcp filtered unknown       no-response
24432/tcp filtered unknown       no-response
31639/tcp filtered unknown       no-response
35640/tcp filtered unknown       no-response
35942/tcp filtered unknown       no-response
36524/tcp filtered febooti-aw    no-response
41987/tcp filtered unknown       no-response
42236/tcp filtered unknown       no-response
43049/tcp filtered unknown       no-response
47001/tcp open     http          syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-title: Not Found
|_http-server-header: Microsoft-HTTPAPI/2.0
49179/tcp filtered unknown       no-response
49664/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49665/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49666/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49667/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49668/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
49669/tcp open     msrpc         syn-ack ttl 125 Microsoft Windows RPC
50650/tcp filtered unknown       no-response
53013/tcp filtered unknown       no-response
63451/tcp filtered unknown       no-response
64320/tcp filtered unknown       no-response
Device type: firewall
Running (JUST GUESSING): Fortinet embedded (86%)
Aggressive OS guesses: Fortinet FortiGate-50B or 310B firewall (86%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=38459%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:480%P=aarch64-unknown-linux-gnu)SEQ()ECN(R=N)T1(R=N)T2(R=N)T3(R=N)T4(R=N
OS:)T4(R=Y%DF=Y%T=80%W=1FFE%S=O%A=O%F=AP%O=NNT11%RD=0%Q=)T4(R=Y%DF=Y%T=80%W
OS:=2000%S=O%A=O%F=AP%O=NNT11%RD=0%Q=)T5(R=N)T5(R=Y%DF=Y%TG=80%W=0%S=Z%A=S+
OS:%F=AR%O=%RD=0%Q=)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T7
OS:(R=N)U1(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=7447
OS:%RUD=G)IE(R=N)

Network Distance: 4 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 62732/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 51162/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 54655/udp): CLEAN (Timeout)
|   Check 4 (port 8612/udp): CLEAN (Failed to receive data)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
|_clock-skew: mean: 0s, deviation: 0s, median: 0s
| smb2-time: 
|   date: 2024-04-03T04:00:58
|_  start_date: N/A
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE (using port 587/tcp)
HOP RTT      ADDRESS
1   73.01 ms 192.168.45.1
2   72.90 ms 192.168.45.254
3   76.97 ms 192.168.251.1
4   77.52 ms 192.168.224.249

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:01:04 2024 -- 1 IP address (1 host up) scanned in 264.67 seconds
