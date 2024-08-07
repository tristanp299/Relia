```bash
nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sU -A --top-ports 100 -oN "/home/kali/Documents/Relia/results/192.168.197.191/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.197.191/scans/xml/_top_100_udp_nmap.xml" 192.168.197.191
```

[/home/kali/Documents/Relia/results/192.168.197.191/scans/_top_100_udp_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.197.191/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Wed Aug  7 22:16:28 2024 as: nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sU -A --top-ports 100 -oN /home/kali/Documents/Relia/results/192.168.197.191/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.197.191/scans/xml/_top_100_udp_nmap.xml 192.168.197.191
Nmap scan report for ip-192-168-197-191.us-west-1.compute.internal (192.168.197.191)
Host is up, received user-set.
Scanned at 2024-08-07 22:16:28 UTC for 1825s
All 100 scanned ports on ip-192-168-197-191.us-west-1.compute.internal (192.168.197.191) are in ignored states.
Not shown: 100 open|filtered udp ports (no-response)
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=8/7%OT=%CT=%CU=%PV=Y%G=N%TM=66B3F95D%P=x86_64-pc-linux-gnu)
SEQ()
U1(R=N)
IE(R=N)


TRACEROUTE (using proto 1/icmp)
HOP RTT      ADDRESS
1   65.81 ms ip-192-168-45-1.us-west-1.compute.internal (192.168.45.1)
2   65.79 ms ip-192-168-45-254.us-west-1.compute.internal (192.168.45.254)
3   66.64 ms ip-192-168-251-1.us-west-1.compute.internal (192.168.251.1)
4   ... 30

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Wed Aug  7 22:46:53 2024 -- 1 IP address (1 host up) scanned in 1825.24 seconds

```
