# Nmap 7.94SVN scan initiated Tue Apr  2 21:10:42 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 49668 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp49668/tcp_49668_rpc_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp49668/xml/tcp_49668_rpc_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.092s latency).
Scanned at 2024-04-02 21:10:43 PDT for 75s

PORT      STATE SERVICE REASON          VERSION
49668/tcp open  msrpc   syn-ack ttl 125 Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:11:58 2024 -- 1 IP address (1 host up) scanned in 76.17 seconds
