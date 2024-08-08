 Nmap 7.94SVN scan initiated Tue Apr  2 21:05:12 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 14020 "--script=banner,(ftp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp14020/tcp_14020_ftp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp14020/xml/tcp_14020_ftp_nmap.xml 192.168.224.247
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.074s latency).
Scanned at 2024-04-02 21:05:12 PDT for 14s

PORT      STATE SERVICE REASON          VERSION
14020/tcp open  ftp     syn-ack ttl 125 FileZilla ftpd
| banner: 220 RELIA FTP Server for DEV resources. Please contact your man
|_ager for access.
|_ftp-bounce: bounce working!
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
|_-r--r--r-- 1 ftp ftp         237639 Nov 04  2022 umbraco.pdf
| ftp-syst: 
|_  SYST: UNIX emulated by FileZilla
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:05:26 2024 -- 1 IP address (1 host up) scanned in 14.33 seconds
