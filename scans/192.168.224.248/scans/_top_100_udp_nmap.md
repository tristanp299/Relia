# Nmap 7.94SVN scan initiated Tue Apr  2 20:56:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/xml/_top_100_udp_nmap.xml 192.168.224.248
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.078s latency).
Scanned at 2024-04-02 20:56:40 PDT for 1243s
Not shown: 99 open|filtered udp ports (no-response)
PORT    STATE  SERVICE REASON               VERSION
515/udp closed printer port-unreach ttl 125
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose
Running: Microsoft Windows 2008, Novell NetWare 6.X
OS CPE: cpe:/o:microsoft:windows_server_2008:r2:sp1 cpe:/o:novell:netware:6.5
OS details: Microsoft Windows Server 2008 R2 SP1, Novell NetWare 6.5
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=4/2%OT=%CT=%CU=515%PV=Y%DS=4%DC=T%G=N%TM=660CD853%P
OS:=aarch64-unknown-linux-gnu)SEQ()T5(R=Y%DF=Y%TG=80%W=0%S=Z%A=S+%F=AR%O=%R
OS:D=0%Q=)U1(R=N)IE(R=N)

Network Distance: 4 hops

TRACEROUTE (using port 515/udp)
HOP RTT      ADDRESS
1   81.46 ms 192.168.45.1
2   81.45 ms 192.168.45.254
3   84.70 ms 192.168.251.1
4   72.96 ms 192.168.224.248

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:17:23 2024 -- 1 IP address (1 host up) scanned in 1243.92 seconds
