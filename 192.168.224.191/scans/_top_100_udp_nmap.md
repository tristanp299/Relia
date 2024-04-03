# Nmap 7.94SVN scan initiated Tue Apr  2 21:01:24 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.224.191/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.191/scans/xml/_top_100_udp_nmap.xml 192.168.224.191
adjust_timeouts2: packet supposedly had rtt of -553490 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -553490 microseconds.  Ignoring time.
Nmap scan report for 192.168.224.191
Host is up, received user-set (0.081s latency).
Scanned at 2024-04-02 21:01:24 PDT for 1350s
Not shown: 99 open|filtered udp ports (no-response)
PORT    STATE  SERVICE      REASON               VERSION
445/udp closed microsoft-ds port-unreach ttl 125
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing an open TCP port so results incomplete
Aggressive OS guesses: Linux 2.6.18 (92%), Linux 2.6.30 (92%), Microsoft Windows Server 2008 R2 (91%), Microsoft Windows Server 2008 R2 SP1 (91%), Microsoft Windows Server 2008 SP2 Datacenter Version (91%), Microsoft Windows Server 2012 Data Center (91%), Microsoft Windows Server 2012 R2 (91%), Microsoft Windows Server 2016 (91%), Microsoft Windows 7 (91%), Microsoft Windows 7 SP1 (91%)
No exact OS matches for host (test conditions non-ideal).
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=4/2%OT=%CT=%CU=445%PV=Y%DS=4%DC=T%G=N%TM=660CD9DA%P=aarch64-unknown-linux-gnu)
SEQ()
T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=FDBD%RUD=G)
IE(R=N)

Network Distance: 4 hops

TRACEROUTE (using port 445/udp)
HOP RTT      ADDRESS
1   75.02 ms 192.168.45.1
2   74.94 ms 192.168.45.254
3   75.97 ms 192.168.251.1
4   75.81 ms 192.168.224.191

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:23:54 2024 -- 1 IP address (1 host up) scanned in 1349.83 seconds
