# Nmap 7.94SVN scan initiated Tue Apr  2 21:08:52 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 143 "--script=banner,(imap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp143/tcp_143_imap_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp143/xml/tcp_143_imap_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.076s latency).
Scanned at 2024-04-02 21:08:52 PDT for 11s

PORT    STATE SERVICE REASON          VERSION
143/tcp open  imap    syn-ack ttl 125 hMailServer imapd
|_imap-capabilities: SORT QUOTA IMAP4 NAMESPACE IMAP4rev1 RIGHTS=texkA0001 CAPABILITY CHILDREN OK completed IDLE ACL
|_banner: * OK IMAPrev1
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:09:03 2024 -- 1 IP address (1 host up) scanned in 10.39 seconds
