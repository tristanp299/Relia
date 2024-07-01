# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:07 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.249/scans/tcp80/tcp_80_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.249/scans/tcp80/xml/tcp_80_http_nmap.xml 192.168.224.249
Nmap scan report for 192.168.224.249
Host is up, received user-set (0.093s latency).
Scanned at 2024-04-02 20:58:08 PDT for 445s

Bug in http-security-headers: no string output.
PORT   STATE SERVICE REASON          VERSION
80/tcp open  http    syn-ack ttl 125 Microsoft IIS httpd 10.0
|_http-devframework: ASP.NET detected. Found related header.
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-dombased-xss: Couldn't find any DOM based XSS.
| http-php-version: Logo query returned unknown hash 242c23ea412530c7d94b77a7a978c176
|_Credits query returned unknown hash 242c23ea412530c7d94b77a7a978c176
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
| http-headers: 
|   Content-Length: 703
|   Content-Type: text/html
|   Last-Modified: Tue, 11 Oct 2022 08:08:24 GMT
|   Accept-Ranges: bytes
|   ETag: "766ac5a248ddd81:0"
|   Server: Microsoft-IIS/10.0
|   X-Powered-By: ASP.NET
|   Date: Wed, 03 Apr 2024 03:58:17 GMT
|   Connection: close
|   
|_  (Request type: HEAD)
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-referer-checker: Couldn't find any cross-domain scripts.
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1; png: 1
|   Longest directory structure:
|     Depth: 0
|     Dir: /
|   Total files found (by extension):
|_    Other: 1; png: 1
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
|_http-mobileversion-checker: No mobile version detected.
| http-vhosts: 
| 15 names had status ERROR
|_113 names had status 200
|_http-malware-host: Host appears to be clean
|_http-server-header: Microsoft-IIS/10.0
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-chrono: Request times for /; avg: 206.24ms; min: 203.53ms; max: 209.17ms
| http-methods: 
|_  Supported Methods: GET
|_http-feed: Couldn't find any feeds.
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-errors: Couldn't find any error pages.
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.249
|     
|     Path: http://192.168.224.249:80/
|     Line number: 7
|     Comment: 
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|         
|_        -->
|_http-title: IIS Windows Server
| http-useragent-tester: 
|   Status for browser useragent: 200
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
|     libcurl-agent/1.0
|     PHP/
|     Python-urllib/2.5
|     GT::WWW
|     Snoopy
|     HTTP::Lite
|     PHPCrawl
|     URI::Fetch
|     PECL::HTTP
|     Wget/1.13.4 (linux-gnu)
|_    WWW-Mechanize/1.34
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:05:33 2024 -- 1 IP address (1 host up) scanned in 445.48 seconds
