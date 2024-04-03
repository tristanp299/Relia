# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:55 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 21 "--script=banner,(ftp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp21/tcp_21_ftp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp21/xml/tcp_21_ftp_nmap.xml 192.168.224.245
Nmap scan report for 192.168.224.245
Host is up, received user-set (0.085s latency).
Scanned at 2024-04-02 20:58:55 PDT for 18s

PORT   STATE SERVICE REASON         VERSION
21/tcp open  ftp     syn-ack ttl 61 vsftpd 2.0.8 or later
|_banner: 220 RELIA Edge FTP server.
Service Info: Host: RELIA

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:59:13 2024 -- 1 IP address (1 host up) scanned in 18.85 seconds
