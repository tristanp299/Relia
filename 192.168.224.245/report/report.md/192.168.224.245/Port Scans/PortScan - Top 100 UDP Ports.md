```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/xml/_top_100_udp_nmap.xml" 192.168.224.245
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/_top_100_udp_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:55 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/xml/_top_100_udp_nmap.xml 192.168.224.245
adjust_timeouts2: packet supposedly had rtt of -368184 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -368184 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.245
Host is up, received user-set (0.082s latency).
Scanned at 2024-04-02 20:58:55 PDT for 673s
Not shown: 94 open|filtered udp ports (no-response)
PORT      STATE  SERVICE         REASON              VERSION
139/udp   closed netbios-ssn     port-unreach ttl 61
177/udp   closed xdmcp           port-unreach ttl 61
1022/udp  closed exp2            port-unreach ttl 61
5000/udp  closed upnp            port-unreach ttl 61
20031/udp closed bakbonenetvault port-unreach ttl 61
65024/udp closed unknown         port-unreach ttl 61
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing an open TCP port so results incomplete
Aggressive OS guesses: Linux 2.6.18 (96%), Linux 2.6.30 (96%), Linux 2.6.28 (95%), Linux 2.6.24 (Palm Pre mobile phone) (94%), Avocent DSR1021 KVM switch (93%), Buffalo TeraStation Pro II NAS device (93%), Dish Network Hopper media device (93%), Android 4.0 (93%), Kyocera CopyStar CS-2560 printer (93%), Linux 3.5 (93%)
No exact OS matches for host (test conditions non-ideal).
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=4/2%OT=%CT=%CU=139%PV=Y%DS=9%DC=T%G=N%TM=660CD6A0%P=aarch64-unknown-linux-gnu)
SEQ()
SEQ(II=I)
T1(R=Y%DF=Y%T=40%S=O%A=O%F=AP%RD=0%Q=)
T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=4EDC%RUD=G)
IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 9 hops

TRACEROUTE (using port 139/udp)
HOP RTT      ADDRESS
1   73.04 ms 192.168.45.1
2   73.03 ms 192.168.45.254
3   73.31 ms 192.168.251.1
4   ... 8
9   90.18 ms 192.168.224.245

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:10:08 2024 -- 1 IP address (1 host up) scanned in 673.26 seconds

```
