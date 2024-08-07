# Nmap 7.94SVN scan initiated Tue Apr  2 21:10:40 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 49666 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp49666/tcp_49666_rpc_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp49666/xml/tcp_49666_rpc_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.086s latency).
Scanned at 2024-04-02 21:10:40 PDT for 44s

PORT      STATE SERVICE REASON          VERSION
49666/tcp open  unknown syn-ack ttl 125

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:11:24 2024 -- 1 IP address (1 host up) scanned in 43.84 seconds
