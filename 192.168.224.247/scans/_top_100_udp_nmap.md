# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/xml/_top_100_udp_nmap.xml 192.168.224.247
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.077s latency).
Scanned at 2024-04-02 20:56:40 PDT for 1256s
All 100 scanned ports on 192.168.224.247 are in ignored states.
Not shown: 100 open|filtered udp ports (no-response)
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing an open TCP port so results incomplete
Aggressive OS guesses: Linux 2.6.18 (92%), Linux 2.6.30 (92%), Microsoft Windows Server 2008 R2 (91%), Microsoft Windows Server 2008 R2 SP1 (91%), Microsoft Windows Server 2008 SP2 Datacenter Version (91%), Microsoft Windows Server 2012 Data Center (91%), Microsoft Windows Server 2012 R2 (91%), Microsoft Windows Server 2016 (91%), Microsoft Windows 7 (91%), Microsoft Windows 7 SP1 (91%)
No exact OS matches for host (test conditions non-ideal).
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=4/2%OT=%CT=%CU=32217%PV=Y%DS=4%DC=T%G=N%TM=660CD860%P=aarch64-unknown-linux-gnu)
SEQ()
T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=9058%RUD=G)
IE(R=N)

Network Distance: 4 hops

TRACEROUTE (using proto 1/icmp)
HOP RTT      ADDRESS
1   71.95 ms 192.168.45.1
2   71.90 ms 192.168.45.254
3   74.27 ms 192.168.251.1
4   74.36 ms 192.168.224.247

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:17:36 2024 -- 1 IP address (1 host up) scanned in 1256.50 seconds
