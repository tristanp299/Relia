# Nmap 7.94SVN scan initiated Tue Apr  2 20:57:13 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/xml/tcp_80_http_nmap.xml 192.168.224.246
Nmap scan report for 192.168.224.246
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 20:57:13 PDT for 240s

Bug in http-security-headers: no string output.
PORT   STATE SERVICE REASON         VERSION
80/tcp open  http    syn-ack ttl 61 Apache httpd 2.4.52
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-title: Code Validation
|_http-date: Wed, 03 Apr 2024 03:58:09 GMT; -23s from local time.
|_http-feed: Couldn't find any feeds.
|_http-mobileversion-checker: No mobile version detected.
|_http-fetch: Please enter the complete path of the directory to save data in.
| http-useragent-tester: 
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
|     libcurl-agent/1.0
|     PHP/
|     Python-urllib/2.5
|     GT::WWW
|     Snoopy
|     MFC_Tear_Sample
|     HTTP::Lite
|     PHPCrawl
|     URI::Fetch
|     Zend_Http_Client
|     http client
|     PECL::HTTP
|   Change in Status Code: 
|     Wget/1.13.4 (linux-gnu): 200
|_    WWW-Mechanize/1.34: 200
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1
|     /css/
|       css: 1
|     /js/
|       js: 1
|   Longest directory structure:
|     Depth: 1
|     Dir: /js/
|   Total files found (by extension):
|_    Other: 1; css: 1; js: 1
| http-errors: 
| Spidering limited to: maxpagecount=40; withinhost=192.168.224.246
|   Found the following error pages: 
|   
|   Error Code: 404
|_  	http://192.168.224.246:80/css/styles.css
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
|_http-referer-checker: Couldn't find any cross-domain scripts.
| http-fileupload-exploiter: 
|   
|_    Couldn't find a file-type field.
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
| http-vhosts: 
| 111 names had status ERROR
|_17 names had status 200
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.246
|     
|     Path: http://192.168.224.246:80/
|     Line number: 14
|     Comment: 
|_        <!-- <link rel="stylesheet" href="css/styles.css" /> -->
| http-headers: 
|   Date: Wed, 03 Apr 2024 03:58:09 GMT
|   Server: Apache/2.4.52 (Ubuntu)
|   Vary: Accept-Encoding
|   Content-Length: 1516
|   Connection: close
|   Content-Type: text/html; charset=UTF-8
|   
|_  (Request type: GET)
| http-php-version: Logo query returned unknown hash d8125ab4ffbb65a15439894308f4c64d
|_Credits query returned unknown hash 67d294c2ea9f2a3b1215f3358e6603ce
|_http-malware-host: Host appears to be clean
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-chrono: Request times for /; avg: 16393.01ms; min: 1994.41ms; max: 25276.38ms
Service Info: Host: 127.0.1.1

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:01:13 2024 -- 1 IP address (1 host up) scanned in 240.06 seconds
