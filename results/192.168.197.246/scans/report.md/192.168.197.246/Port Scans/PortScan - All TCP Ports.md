```bash
nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/kali/Documents/Relia/results/192.168.197.246/scans/_full_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.197.246/scans/xml/_full_tcp_nmap.xml" 192.168.197.246
```

[/home/kali/Documents/Relia/results/192.168.197.246/scans/_full_tcp_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.197.246/scans/_full_tcp_nmap.txt):

```
# Nmap 7.94SVN scan initiated Wed Aug  7 21:46:02 2024 as: nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN /home/kali/Documents/Relia/results/192.168.197.246/scans/_full_tcp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.197.246/scans/xml/_full_tcp_nmap.xml 192.168.197.246
Nmap scan report for ip-192-168-197-246.us-west-1.compute.internal (192.168.197.246)
Host is up, received user-set.
Scanned at 2024-08-07 21:46:02 UTC for 283s
All 65535 scanned ports on ip-192-168-197-246.us-west-1.compute.internal (192.168.197.246) are in ignored states.
Not shown: 65535 filtered tcp ports (no-response)
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.94SVN%E=4%D=8/7%OT=%CT=%CU=%PV=Y%G=N%TM=66B3EC35%P=x86_64-pc-linux-gnu)
SEQ()
U1(R=N)
IE(R=N)


TRACEROUTE (using proto 1/icmp)
HOP RTT      ADDRESS
1   65.84 ms ip-192-168-45-1.us-west-1.compute.internal (192.168.45.1)
2   65.82 ms ip-192-168-45-254.us-west-1.compute.internal (192.168.45.254)
3   66.62 ms ip-192-168-251-1.us-west-1.compute.internal (192.168.251.1)
4   ... 30

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Wed Aug  7 21:50:45 2024 -- 1 IP address (1 host up) scanned in 283.35 seconds

```
