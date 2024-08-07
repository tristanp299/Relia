# Nmap 7.94SVN scan initiated Tue Apr  2 21:09:01 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 587 "--script=banner,(smtp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp587/tcp_587_smtp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp587/xml/tcp_587_smtp_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 21:09:01 PDT for 23s

PORT    STATE SERVICE REASON          VERSION
587/tcp open  smtp    syn-ack ttl 125 hMailServer smtpd
|_banner: 220 MAIL ESMTP
| smtp-vuln-cve2010-4344: 
|_  The SMTP server is not Exim: NOT VULNERABLE
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
Service Info: Host: MAIL; OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:09:24 2024 -- 1 IP address (1 host up) scanned in 22.76 seconds
