# Nmap 7.94SVN scan initiated Tue Apr  2 21:05:27 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/192.168.224.250/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.250/scans/xml/_quick_tcp_nmap.xml 192.168.224.250
adjust_timeouts2: packet supposedly had rtt of -200736 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -200736 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -198926 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -198926 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -300568 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -300568 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -302217 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -302217 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -316442 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -316442 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -271618 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -271618 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.250
Host is up, received user-set (0.083s latency).
Scanned at 2024-04-02 21:05:27 PDT for 212s
Not shown: 996 closed tcp ports (reset)
PORT     STATE SERVICE            REASON          VERSION
135/tcp  open  msrpc              syn-ack ttl 125 Microsoft Windows RPC
139/tcp  open  netbios-ssn        syn-ack ttl 125 Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?      syn-ack ttl 125
3389/tcp open  ssl/ms-wbt-server? syn-ack ttl 125
| rdp-ntlm-info: 
|   Target_Name: WINPREP
|   NetBIOS_Domain_Name: WINPREP
|   NetBIOS_Computer_Name: WINPREP
|   DNS_Domain_Name: WINPREP
|   DNS_Computer_Name: WINPREP
|   Product_Version: 10.0.22000
|_  System_Time: 2024-04-03T04:08:45+00:00
| ssl-cert: Subject: commonName=WINPREP
| Issuer: commonName=WINPREP
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-03-07T05:25:18
| Not valid after:  2024-09-06T05:25:18
| MD5:   51fe:9a6b:977e:78b5:d2d2:35a0:4b19:cb0a
| SHA-1: 9ec8:635a:9ebb:0933:560e:50e5:16ed:948c:4b98:430d
| -----BEGIN CERTIFICATE-----
| MIIC0jCCAbqgAwIBAgIQVyQ8hwp5ja5On/WxoMbIQzANBgkqhkiG9w0BAQsFADAS
| MRAwDgYDVQQDEwdXSU5QUkVQMB4XDTI0MDMwNzA1MjUxOFoXDTI0MDkwNjA1MjUx
| OFowEjEQMA4GA1UEAxMHV0lOUFJFUDCCASIwDQYJKoZIhvcNAQEBBQADggEPADCC
| AQoCggEBALgBTSknRu2n0JD9KIyDYjk/bFfD5N7iY4IQ6/+tgkzTO7N3LfpMn0iB
| y4El/3mwFEZk58RSrbxfbuBmKTN7U3k1skhoOt7tK557/Nbl81M/YM2QqzmT8Kho
| WHXLo5bI1ePY+VZHkgLBvWuNohutkcLnnADFO/9YvaWorPBcB43T6630cfPCLYJC
| xTSXOYKMmVG/mu79fbwZDng44QmAKGJjIpmU9a+OJCZEsHE5DwMav+V2HWjiUrU4
| 47JdUqOMpetrPp/BsE4ztCBlD5qXVQAycNYzjyXCtu//DwpZfNhS+RExkxjX34X9
| syVhpIJnvsfOdKFwH5lBIzf1YrT2dd0CAwEAAaMkMCIwEwYDVR0lBAwwCgYIKwYB
| BQUHAwEwCwYDVR0PBAQDAgQwMA0GCSqGSIb3DQEBCwUAA4IBAQB2BaKxWEpYJ+Lb
| slcgSZcKq+NHYZMYexA8Ip+1j44zsAKdfH3cfTEh3gMGNxjWRuW7K0Zr2/enIcKW
| LmyH7M2Nqz3c9+g7jR7Rt8uhniHVrF59A0fMw+HTEs9ofDIFU92ap1Yn/bx51cC3
| ITCXykxjDvnb4oiqkIMolps3fC71Y4+f9TXeHoOMSoJ0PQqS9eqC/bnWanpWhTVQ
| LGGGTk071eHTvP5jxUOe/nqDs5HYzqktcp3DAf7QtcL38a0csZmMFg6MWrMTcdWB
| jsx1a0FUIf9Qk+00n7dlipCnT7MwGqMwH6n1njs/Zsvkh90oRgE5Ett95gX3L5B9
| KiBcAO4P
|_-----END CERTIFICATE-----
|_ssl-date: 2024-04-03T04:08:57+00:00; 0s from scanner time.
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows 11|10|2008 (88%), FreeBSD 6.X (85%)
OS CPE: cpe:/o:freebsd:freebsd:6.2 cpe:/o:microsoft:windows_10 cpe:/o:microsoft:windows_server_2008
Aggressive OS guesses: Microsoft Windows 11 21H2 (88%), FreeBSD 6.2-RELEASE (85%), Microsoft Windows 10 (85%), Microsoft Windows Server 2008 (85%)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=135%CT=1%CU=37069%PV=Y%DS=4%DC=T%G=Y%TM=660C
OS:D65B%P=aarch64-unknown-linux-gnu)SEQ(TS=A)SEQ(SP=106%GCD=1%ISR=10A%TS=A)
OS:SEQ(SP=FE%GCD=1%ISR=108%TI=RD%TS=C)SEQ(SP=FF%GCD=1%ISR=109%TS=A)OPS(O1=M
OS:551NW8ST11%O2=M551NW8ST11%O3=M551NW8NNT11%O4=M551NW8ST11%O5=M551NW8ST11%
OS:O6=M551ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FFDC)ECN(R=N)
OS:ECN(R=Y%DF=Y%T=80%W=FFFF%O=M551NW8NNS%CC=N%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+%
OS:F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=N)T5(R=N)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F
OS:=AR%O=%RD=0%Q=)T6(R=N)T7(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%
OS:RIPCK=G%RUCK=9322%RUD=G)IE(R=N)

Uptime guess: 0.003 days (since Tue Apr  2 21:05:02 2024)
Network Distance: 4 hops
TCP Sequence Prediction: Difficulty=254 (Good luck!)
IP ID Sequence Generation: Randomized
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 25404/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 37595/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 55819/udp): CLEAN (Failed to receive data)
|   Check 4 (port 16210/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
| smb2-time: 
|   date: 2024-04-03T04:08:47
|_  start_date: N/A
|_clock-skew: mean: 0s, deviation: 0s, median: 0s

TRACEROUTE (using port 80/tcp)
HOP RTT       ADDRESS
1   100.17 ms 192.168.45.1
2   72.29 ms  192.168.45.254
3   75.24 ms  192.168.251.1
4   75.28 ms  192.168.224.250

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:08:59 2024 -- 1 IP address (1 host up) scanned in 212.51 seconds
