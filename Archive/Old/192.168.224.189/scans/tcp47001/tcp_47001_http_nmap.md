# Nmap 7.94SVN scan initiated Tue Apr  2 21:10:15 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 47001 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp47001/tcp_47001_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.189/scans/tcp47001/xml/tcp_47001_http_nmap.xml 192.168.224.189
Nmap scan report for 192.168.224.189
Host is up, received user-set (0.092s latency).
Scanned at 2024-04-02 21:10:15 PDT for 27s

PORT      STATE SERVICE REASON          VERSION
47001/tcp open  winrm?  syn-ack ttl 125
| fingerprint-strings: 
|   JavaRMI: 
|     HTTP/1.1 400 Bad Request
|     Content-Type: text/html; charset=us-ascii
|     Server: Microsoft-HTTPAPI/2.0
|     Date: Wed, 03 Apr 2024 04:10:23 GMT
|     Connection: close
|     Content-Length: 326
|     <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN""http://www.w3.org/TR/html4/strict.dtd">
|     <HTML><HEAD><TITLE>Bad Request</TITLE>
|     <META HTTP-EQUIV="Content-Type" Content="text/html; charset=us-ascii"></HEAD>
|     <BODY><h2>Bad Request - Invalid Verb</h2>
|     <hr><p>HTTP Error 400. The request verb is invalid.</p>
|_    </BODY></HTML>
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port47001-TCP:V=7.94SVN%I=7%D=4/2%Time=660CD6AF%P=aarch64-unknown-linux
SF:-gnu%r(JavaRMI,1F9,"HTTP/1\.1\x20400\x20Bad\x20Request\r\nContent-Type:
SF:\x20text/html;\x20charset=us-ascii\r\nServer:\x20Microsoft-HTTPAPI/2\.0
SF:\r\nDate:\x20Wed,\x2003\x20Apr\x202024\x2004:10:23\x20GMT\r\nConnection
SF::\x20close\r\nContent-Length:\x20326\r\n\r\n<!DOCTYPE\x20HTML\x20PUBLIC
SF:\x20\"-//W3C//DTD\x20HTML\x204\.01//EN\"\"http://www\.w3\.org/TR/html4/
SF:strict\.dtd\">\r\n<HTML><HEAD><TITLE>Bad\x20Request</TITLE>\r\n<META\x2
SF:0HTTP-EQUIV=\"Content-Type\"\x20Content=\"text/html;\x20charset=us-asci
SF:i\"></HEAD>\r\n<BODY><h2>Bad\x20Request\x20-\x20Invalid\x20Verb</h2>\r\
SF:n<hr><p>HTTP\x20Error\x20400\.\x20The\x20request\x20verb\x20is\x20inval
SF:id\.</p>\r\n</BODY></HTML>\r\n");

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:10:42 2024 -- 1 IP address (1 host up) scanned in 26.87 seconds
