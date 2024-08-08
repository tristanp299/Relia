```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/kali/Documents/Relia/results/192.168.224.246/scans/_full_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.246/scans/xml/_full_tcp_nmap.xml" 192.168.224.246
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/_full_tcp_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/_full_tcp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:57:13 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN /home/kali/Documents/Relia/results/192.168.224.246/scans/_full_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.246/scans/xml/_full_tcp_nmap.xml 192.168.224.246
Increasing send delay for 192.168.224.246 from 5 to 10 due to 27 out of 67 dropped probes since last increase.
Warning: 192.168.224.246 giving up on port because retransmission cap hit (6).
adjust_timeouts2: packet supposedly had rtt of -366503 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -366503 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -366924 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -366924 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -372052 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -372052 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -423292 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -423292 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -430142 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -430142 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -426554 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -426554 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -1196225 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -1196225 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -666847 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -666847 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -253355 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -253355 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.246
Host is up, received user-set (0.079s latency).
Scanned at 2024-04-02 20:57:13 PDT for 229s
Not shown: 65512 closed tcp ports (reset)
PORT      STATE    SERVICE        REASON         VERSION
80/tcp    open     http           syn-ack ttl 61 Apache httpd 2.4.52
|_http-server-header: Apache/2.4.52 (Ubuntu)
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Code Validation
443/tcp   open     ssl/https      syn-ack ttl 61
| http-methods: 
|_  Supported Methods: HEAD POST OPTIONS
|_http-server-header: Apache/2.4.52 (Ubuntu)
| ssl-cert: Subject: commonName=demo
| Subject Alternative Name: DNS:demo
| Issuer: commonName=demo
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2022-10-12T07:46:27
| Not valid after:  2032-10-09T07:46:27
| MD5:   6361:be08:5259:3a75:cd26:f869:1614:3c94
| SHA-1: 8fa0:04a7:5d03:4c29:44b7:6b14:119f:fd79:3c7e:5093
| -----BEGIN CERTIFICATE-----
| MIIC6TCCAdGgAwIBAgIUIN3Z/giwrWikVN/gzzofa98CJ1AwDQYJKoZIhvcNAQEL
| BQAwDzENMAsGA1UEAwwEZGVtbzAeFw0yMjEwMTIwNzQ2MjdaFw0zMjEwMDkwNzQ2
| MjdaMA8xDTALBgNVBAMMBGRlbW8wggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEK
| AoIBAQCMPw2+IkC55uip8gDmvy+mN/FtQJBck6audIht6POsdrE2GzfhAoxZY9al
| XkTc3WPOxP2X1I4ea1t1y8SQuX7jomUlNOgkGtVbj+RYzU8Qau7XWSTBMbVkRluc
| B+w5vPsGL1XGMd35V7Td6ZhotXLwc0j19smwewETujURfSmGCKdwbHztKozyW9Qg
| QFOtNI4gOHpvMxTYpR3QDkBYvIzaH+FaU8xqrr/GJiFSz8MUhxVPSM2QyqSmsFyE
| HYijIDbxBNRyf1lAmReLdwpwGqpRvBF1wYfpYyTvjW/j0LQPfvCcCVxD1v/3N3oK
| VR4/EYqBrCr9umF7Q3w5E4hC0x5VAgMBAAGjPTA7MAkGA1UdEwQCMAAwDwYDVR0R
| BAgwBoIEZGVtbzAdBgNVHQ4EFgQUqWpscb2cgQbMGE4Nh4vVDLAs55EwDQYJKoZI
| hvcNAQELBQADggEBACvVHEqW54LzwFNKfLMlbbrSitnXhGc1zgOaYdBnF95weO3j
| 5gEbGNElednFgWQEZzLz5ruS9i0aiKsQYKuh+AL+QQRdycfCbTxDVTopO9sxFYGd
| UpSxCGToYe5JULiNpnBpTWPEldc608y2jhpJpsH5UGifvRp/VpHW/3A+9t8oAUeN
| /SVW3bQ7sLEEvCmHH4E1uJS3k6kBidDY1A9OOxaL0k2v/cB8PONnEMwP4DcmKRA1
| cVrgXiR8x7E5zcVUPj8cM5+DqSOQTAphAcVbVx2c/K2XMENFZqVUbRFbuZSXVExp
| TQICNlWeutzCZGE7rREsIUUIigT9erEAvTu28RI=
|_-----END CERTIFICATE-----
| tls-alpn: 
|_  http/1.1
|_ssl-date: TLS randomness does not represent time
|_http-title: Code Validation
2186/tcp  filtered gtaua          no-response
2222/tcp  open     ssh            syn-ack ttl 61 OpenSSH 8.9p1 Ubuntu 3 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   256 42:2d:8d:48:ad:10:dd:ff:70:25:8b:46:2e:5c:ff:1d (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBEpVNr/0MSfOq95rNQVnUXG+NF7yHDkPeFEXylLHxnZSqLAEqWi+z67gxHF0QVSjtaeEVbOnind7C3LKLGe1b8g=
|   256 aa:4a:c3:27:b1:19:30:d7:63:91:96:ae:63:3c:07:dc (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIFcUmhqn+iJNZi0wDswh/Jusg6ZX0SGGoKcsNCB69vQA
2701/tcp  filtered sms-rcinfo     no-response
3188/tcp  filtered brcm-comm-port no-response
7495/tcp  filtered unknown        no-response
7844/tcp  filtered unknown        no-response
8040/tcp  filtered ampify         no-response
16719/tcp filtered unknown        no-response
17292/tcp filtered unknown        no-response
18172/tcp filtered unknown        no-response
21361/tcp filtered unknown        no-response
39652/tcp filtered unknown        no-response
42783/tcp filtered unknown        no-response
47977/tcp filtered unknown        no-response
52276/tcp filtered unknown        no-response
52567/tcp filtered unknown        no-response
56051/tcp filtered unknown        no-response
58036/tcp filtered unknown        no-response
61064/tcp filtered unknown        no-response
63242/tcp filtered unknown        no-response
64730/tcp filtered unknown        no-response
Aggressive OS guesses: Linux 2.6.32 (87%), Linux 2.6.32 or 3.10 (87%), Linux 2.6.39 (87%), Linux 3.10 - 3.12 (87%), Linux 3.4 (87%), Linux 3.5 (87%), Linux 4.2 (87%), Linux 4.4 (87%), Synology DiskStation Manager 5.1 (87%), WatchGuard Fireware 11.8 (87%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=80%CT=1%CU=35346%PV=Y%DS=4%DC=T%G=Y%TM=660CD
OS:47E%P=aarch64-unknown-linux-gnu)SEQ(TI=Z%TS=A)SEQ(SP=103%GCD=1%ISR=10A%T
OS:I=Z%TS=A)SEQ(SP=103%GCD=1%ISR=10A%TI=Z%TS=C)SEQ(SP=103%GCD=1%ISR=10A%TI=
OS:Z%CI=RI%TS=A)SEQ(SP=FB%GCD=1%ISR=FD%TI=Z%TS=A)OPS(O1=M551ST11NW7%O2=M551
OS:ST11NW7%O3=M551NNT11NW7%O4=M551ST11NW7%O5=M551ST11NW7%O6=M551ST11)OPS(O1
OS:=M551ST11NW7%O2=M551ST11NW7%O3=M551NNT11NW7%O4=NNT11%O5=M551ST11NW7%O6=M
OS:551ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=1F8%W5=FE88%W6=FE88)WIN(W1=FE88%W
OS:2=FE88%W3=FE88%W4=FE88%W5=FE88%W6=FE88)ECN(R=N)ECN(R=Y%DF=Y%T=40%W=FAF0%
OS:O=M551NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=
OS:N)T4(R=N)T5(R=N)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=N)T7(
OS:R=N)T7(R=Y%DF=Y%T=40%W=1F8%S=O%A=O%F=A%O=NNT11%RD=0%Q=)U1(R=Y%DF=N%T=40%
OS:IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=A9F6%RUD=G)IE(R=Y%DFI=N%T=40%CD=S
OS:)

Uptime guess: 8.936 days (since Sun Mar 24 22:33:04 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=259 (Good luck!)
IP ID Sequence Generation: All zeros
Service Info: Host: 127.0.1.1; OS: Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE (using port 3306/tcp)
HOP RTT      ADDRESS
1   74.95 ms 192.168.45.1
2   74.93 ms 192.168.45.254
3   84.05 ms 192.168.251.1
4   79.29 ms 192.168.224.246

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:01:02 2024 -- 1 IP address (1 host up) scanned in 229.69 seconds

```
