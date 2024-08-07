```bash
nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sU -A --top-ports 100 -oN "/home/kali/Documents/Relia/results/172.16.157.15/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/Relia/results/172.16.157.15/scans/xml/_top_100_udp_nmap.xml" 172.16.157.15
```

[/home/kali/Documents/Relia/results/172.16.157.15/scans/_top_100_udp_nmap.txt](file:///home/kali/Documents/Relia/results/172.16.157.15/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Wed Aug  7 22:01:27 2024 as: nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/172.16.157.15/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/172.16.157.15/scans/xml/_top_100_udp_nmap.xml 172.16.157.15
Nmap scan report for ip-172-16-157-15.us-west-1.compute.internal (172.16.157.15)
Host is up, received user-set.
Scanned at 2024-08-07 22:01:27 UTC for 1825s
All 100 scanned ports on ip-172-16-157-15.us-west-1.compute.internal (172.16.157.15) are in ignored states.
Not shown: 100 open|filtered udp ports (no-response)
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=8/7%OT=%CT=%CU=%PV=Y%G=N%TM=66B3F5D8%P=x86_64-pc-linux-gnu)
SEQ()
U1(R=N)
IE(R=N)


TRACEROUTE (using proto 1/icmp)
HOP RTT    ADDRESS
1   ... 30

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Wed Aug  7 22:31:52 2024 -- 1 IP address (1 host up) scanned in 1824.91 seconds

```
