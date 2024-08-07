```bash
nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN "/home/kali/Documents/Relia/results/172.16.157.21/scans/_quick_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/172.16.157.21/scans/xml/_quick_tcp_nmap.xml" 172.16.157.21
```

[/home/kali/Documents/Relia/results/172.16.157.21/scans/_quick_tcp_nmap.txt](file:///home/kali/Documents/Relia/results/172.16.157.21/scans/_quick_tcp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Wed Aug  7 21:46:52 2024 as: nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN /home/kali/Documents/Relia/results/172.16.157.21/scans/_quick_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/172.16.157.21/scans/xml/_quick_tcp_nmap.xml 172.16.157.21
Nmap scan report for ip-172-16-157-21.us-west-1.compute.internal (172.16.157.21)
Host is up, received user-set.
Scanned at 2024-08-07 21:46:52 UTC for 24s
All 1000 scanned ports on ip-172-16-157-21.us-west-1.compute.internal (172.16.157.21) are in ignored states.
Not shown: 1000 filtered tcp ports (no-response)
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=8/7%OT=%CT=%CU=%PV=Y%G=N%TM=66B3EB64%P=x86_64-pc-linux-gnu)
SEQ()
U1(R=N)
IE(R=N)


TRACEROUTE (using proto 1/icmp)
HOP RTT    ADDRESS
1   ... 30

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Wed Aug  7 21:47:16 2024 -- 1 IP address (1 host up) scanned in 24.68 seconds

```
