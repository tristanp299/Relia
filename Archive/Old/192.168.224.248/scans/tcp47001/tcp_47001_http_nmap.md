# Nmap 7.94SVN scan initiated Tue Apr  2 21:02:38 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 47001 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp47001/tcp_47001_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp47001/xml/tcp_47001_http_nmap.xml 192.168.224.248
Nmap scan report for 192.168.224.248
Host is up, received user-set.
Scanned at 2024-04-02 21:02:38 PDT for 1s

PORT      STATE    SERVICE REASON      VERSION
47001/tcp filtered winrm   no-response

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:02:39 2024 -- 1 IP address (1 host up) scanned in 1.37 seconds
