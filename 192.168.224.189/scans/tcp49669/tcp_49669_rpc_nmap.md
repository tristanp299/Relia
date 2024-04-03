# Nmap 7.94SVN scan initiated Tue Apr  2 21:11:25 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 49669 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp49669/tcp_49669_rpc_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp49669/xml/tcp_49669_rpc_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.084s latency).
Scanned at 2024-04-02 21:11:25 PDT for 65s

PORT      STATE SERVICE REASON          VERSION
49669/tcp open  unknown syn-ack ttl 125

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:12:30 2024 -- 1 IP address (1 host up) scanned in 65.23 seconds
