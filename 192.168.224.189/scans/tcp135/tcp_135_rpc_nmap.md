# Nmap 7.94SVN scan initiated Tue Apr  2 21:08:37 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 135 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp135/tcp_135_rpc_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp135/xml/tcp_135_rpc_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set.
Scanned at 2024-04-02 21:08:37 PDT for 1s

PORT    STATE    SERVICE REASON      VERSION
135/tcp filtered msrpc   no-response

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:08:38 2024 -- 1 IP address (1 host up) scanned in 1.42 seconds
