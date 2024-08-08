# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:08 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/xml/_quick_tcp_nmap.xml 192.168.224.245
adjust_timeouts2: packet supposedly had rtt of -203234 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -203234 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -203353 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -203353 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -200491 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -200491 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -238298 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -238298 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -153564 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -153564 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -195623 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -195623 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -211143 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -211143 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -186164 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -186164 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -218810 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -218810 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -683378 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -683378 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -222286 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -222286 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -246881 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -246881 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -1355037 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -1355037 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.245
Host is up, received user-set (0.080s latency).
Scanned at 2024-04-02 20:58:09 PDT for 45s
Not shown: 995 closed tcp ports (reset)
PORT     STATE SERVICE  REASON         VERSION
21/tcp   open  ftp      syn-ack ttl 61 vsftpd 2.0.8 or later
| ftp-syst: 
|   STAT: 
| FTP server status:
|      Connected to 192.168.45.189
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      At session startup, client count was 3
|      vsFTPd 3.0.3 - secure, fast, stable
|_End of status
|_ftp-anon: Anonymous FTP login allowed (FTP code 230)
80/tcp   open  http     syn-ack ttl 61 Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
|_http-title: RELIA Corp.
443/tcp  open  ssl/http syn-ack ttl 61 Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
|_ssl-date: TLS randomness does not represent time
| tls-alpn: 
|_  http/1.1
|_http-title: RELIA Corp.
| ssl-cert: Subject: commonName=web01.relia.com/organizationName=RELIA/stateOrProvinceName=Berlin/countryName=DE/localityName=Munich/organizationalUnitName=IT Department
| Issuer: commonName=web01.relia.com/organizationName=RELIA/stateOrProvinceName=Berlin/countryName=DE/localityName=Munich/organizationalUnitName=IT Department
| Public Key type: rsa
| Public Key bits: 4096
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2022-10-12T08:55:44
| Not valid after:  2032-10-09T08:55:44
| MD5:   fa8f:53d5:841c:47dc:ac0c:8d5a:3acb:43a7
| SHA-1: 9fd6:3372:2dfd:ed09:0915:6b60:2604:b238:f02a:eab7
| -----BEGIN CERTIFICATE-----
| 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
|_-----END CERTIFICATE-----
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
2222/tcp open  ssh      syn-ack ttl 61 OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 30:0c:6c:9b:ac:07:47:5e:df:6d:ff:38:63:38:2a:fd (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCkRPaVboTfq+VZYyf1bsUlg+WZrPP1F6fRrA0TNkHmamfuFAhW9XfCiuh2GOnSkNeGUXLcMAgMtbki6uj4l6vTw5/pqM/jBz00be6Ty+g0CDz9gmb+p0iX+8vCeG6aB0vea9bvkjaABticCS1CmUEbfEe/jCn/11c4NmHleCFfVxE8PBRE2OyVWlFQkkcB74O0FS4AOfbnrAx3pAF4rcd7XsTgi4V1e/sKZ8RIcTlueVdnzZEMcpLeZXUR1cXsJ9zwklFLuMWuUjonYC7BFvT+Bf81jlO1/e9B0RxfalfCfeUthSoa2VGwpfvesCdHl0exvy1PXaeR2XUX5ZJ0jmoP7cvj1rb+ZrnUU/Sie0qpVklHpkjggz0li7Mk4h/CI+est9oeHP+UXVv+Xl/jpnXz/RX/1y03wkTe9Pygxo3NsLdrs22/UCQ5GZ5x78UJQBXCCI93KHY1BG28B9V8xT9PGmpFDgjnF3pFuZoMevmeHSVNBlNQV42/qFCJr48XbAM=
|   256 f3:a9:70:76:c8:d4:c4:17:f4:39:1f:be:58:9d:1f:a5 (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBK6SiUV5zqxqNJ9a/p9l+VpxxqiXnYri40OjXMExS/tP0EbTAEpojn4uXKOgR3oEaMmQVmI9QLPTehCFLNJ3iJo=
|   256 21:a0:79:82:2d:e6:2a:76:11:24:2f:7e:2e:a8:c7:83 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIJ9WPZpl/+VGWtnGi3tQSn1u5FAiDr9bKTV2xCUqje/c
8000/tcp open  http     syn-ack ttl 61 Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
|_http-title: Site doesn't have a title (text/html).
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
Aggressive OS guesses: Linux 2.6.32 (87%), Linux 2.6.32 or 3.10 (87%), Synology DiskStation Manager 5.1 (87%), Linux 2.6.35 (87%), Linux 2.6.39 (86%), Linux 3.10 - 3.12 (86%), Linux 3.4 (86%), Linux 4.4 (86%), WatchGuard Fireware 11.8 (86%), DD-WRT v24-sp1 (Linux 2.4) (86%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=21%CT=1%CU=37038%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:3FE%P=aarch64-unknown-linux-gnu)SEQ(TS=A)SEQ(SP=F9%GCD=1%ISR=10D%TI=Z%TS
OS:=A)SEQ(SP=FA%GCD=1%ISR=10C%TI=Z%TS=A)SEQ(SP=FD%GCD=1%ISR=10C%TI=Z%TS=C)O
OS:PS(O1=M551ST11NW7%O2=M551ST11NW7%O3=M551NNT11NW7%O4=M551ST11NW7%O5=M551S
OS:T11NW7%O6=M551ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6=FE88)E
OS:CN(R=Y%DF=Y%T=40%W=FAF0%O=M551NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%F
OS:=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%R
OS:D=0%Q=)T6(R=N)T7(R=N)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%
OS:RUCK=778F%RUD=G)IE(R=Y%DFI=N%T=40%CD=S)

Uptime guess: 8.048 days (since Mon Mar 25 19:49:12 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=250 (Good luck!)
IP ID Sequence Generation: All zeros
Service Info: Host: RELIA; OS: Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE (using port 110/tcp)
HOP RTT      ADDRESS
1   72.50 ms 192.168.45.1
2   72.45 ms 192.168.45.254
3   72.60 ms 192.168.251.1
4   72.66 ms 192.168.224.245

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:54 2024 -- 1 IP address (1 host up) scanned in 46.42 seconds
