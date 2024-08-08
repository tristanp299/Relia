# Nmap 7.94SVN scan initiated Tue Apr  2 21:07:39 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 49671 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/Relia/results/192.168.224.191/scans/tcp49671/tcp_49671_rpc_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.191/scans/tcp49671/xml/tcp_49671_rpc_nmap.xml 192.168.224.191
Nmap scan report for 192.168.224.191
Host is up, received user-set (0.087s latency).
Scanned at 2024-04-02 21:07:40 PDT for 81s

PORT      STATE SERVICE REASON          VERSION
49671/tcp open  msrpc   syn-ack ttl 125 Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:09:01 2024 -- 1 IP address (1 host up) scanned in 81.60 seconds
