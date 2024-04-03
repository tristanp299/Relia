# Nmap 7.94SVN scan initiated Tue Apr  2 21:08:26 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 110 "--script=banner,(pop3* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp110/tcp_110_pop3_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp110/xml/tcp_110_pop3_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.090s latency).
Scanned at 2024-04-02 21:08:26 PDT for 10s

PORT    STATE SERVICE REASON          VERSION
110/tcp open  pop3    syn-ack ttl 125 hMailServer pop3d
|_banner: +OK POP3
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:08:36 2024 -- 1 IP address (1 host up) scanned in 9.94 seconds
