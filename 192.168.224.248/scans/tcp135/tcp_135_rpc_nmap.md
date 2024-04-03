# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:05 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 135 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp135/tcp_135_rpc_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp135/xml/tcp_135_rpc_nmap.xml 192.168.224.248
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 20:58:06 PDT for 22s

PORT    STATE SERVICE REASON          VERSION
135/tcp open  msrpc   syn-ack ttl 125 Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:28 2024 -- 1 IP address (1 host up) scanned in 22.63 seconds
