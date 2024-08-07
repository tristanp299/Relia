```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN "/home/kali/Documents/Relia/results/192.168.224.246/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.246/scans/xml/_top_100_udp_nmap.xml" 192.168.224.246
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/_top_100_udp_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:06 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.224.246/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.246/scans/xml/_top_100_udp_nmap.xml 192.168.224.246
adjust_timeouts2: packet supposedly had rtt of -64062 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -57629 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -57629 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -76262 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -76262 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -140205 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -140205 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.246
Host is up, received user-set (0.074s latency).
Scanned at 2024-04-02 20:58:06 PDT for 635s
Not shown: 94 open|filtered udp ports (no-response)
PORT      STATE  SERVICE       REASON              VERSION
17/udp    closed qotd          port-unreach ttl 61
445/udp   closed microsoft-ds  port-unreach ttl 61
996/udp   closed vsinet        port-unreach ttl 61
2223/udp  closed rockwell-csp2 port-unreach ttl 61
10000/udp closed ndmp          port-unreach ttl 61
49190/udp closed unknown       port-unreach ttl 61
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose
Running: Linux 2.6.X
OS CPE: cpe:/o:linux:linux_kernel:2.6.18
OS details: Linux 2.6.18, Linux 2.6.30
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=%CT=%CU=17%PV=Y%DS=4%DC=T%G=N%TM=660CD649%P=
OS:aarch64-unknown-linux-gnu)SEQ()T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=
OS:0%Q=)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=3649%RUD=G)
OS:IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 4 hops

TRACEROUTE (using port 445/udp)
HOP RTT      ADDRESS
1   72.64 ms 192.168.45.1
2   72.57 ms 192.168.45.254
3   74.90 ms 192.168.251.1
4   75.36 ms 192.168.224.246

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:08:41 2024 -- 1 IP address (1 host up) scanned in 636.18 seconds

```
