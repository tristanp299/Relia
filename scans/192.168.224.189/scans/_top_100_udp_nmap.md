# Nmap 7.94SVN scan initiated Tue Apr  2 21:04:09 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/xml/_top_100_udp_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.092s latency).
Scanned at 2024-04-02 21:04:09 PDT for 1320s
Not shown: 99 open|filtered udp ports (no-response)
PORT     STATE  SERVICE   REASON               VERSION
1029/udp closed solid-mux port-unreach ttl 125
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose
Running: Microsoft Windows 2008, Novell NetWare 6.X
OS CPE: cpe:/o:microsoft:windows_server_2008:r2:sp1 cpe:/o:novell:netware:6.5
OS details: Microsoft Windows Server 2008 R2 SP1, Novell NetWare 6.5
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=%CT=%CU=1029%PV=Y%DS=8%DC=T%G=N%TM=660CDA61%
OS:P=aarch64-unknown-linux-gnu)SEQ()T5(R=Y%DF=Y%TG=80%W=0%S=Z%A=S+%F=AR%O=%
OS:RD=0%Q=)U1(R=N)IE(R=N)

Network Distance: 8 hops

TRACEROUTE (using port 1029/udp)
HOP RTT       ADDRESS
1   88.21 ms  192.168.45.1
2   ...
3   100.94 ms 192.168.251.1
4   ... 7
8   100.79 ms 192.168.224.189

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:26:09 2024 -- 1 IP address (1 host up) scanned in 1320.31 seconds
