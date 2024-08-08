# Nmap 7.94SVN scan initiated Tue Apr  2 21:01:07 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 47001 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.249/scans/tcp47001/tcp_47001_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.249/scans/tcp47001/xml/tcp_47001_http_nmap.xml 192.168.224.249
Nmap scan report for 192.168.224.249
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 21:01:07 PDT for 461s

Bug in http-security-headers: no string output.
PORT      STATE SERVICE REASON          VERSION
47001/tcp open  http    syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-chrono: Request times for /; avg: 413.75ms; min: 205.71ms; max: 1237.09ms
| http-errors: 
| Spidering limited to: maxpagecount=40; withinhost=192.168.224.249
|   Found the following error pages: 
|   
|   Error Code: 404
|_  	http://192.168.224.249:47001/
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
| http-useragent-tester: 
|   Status for browser useragent: 404
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
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
|     Wget/1.13.4 (linux-gnu)
|_    WWW-Mechanize/1.34
| http-sitemap-generator: 
|   Directory structure:
|   Longest directory structure:
|     Depth: 0
|     Dir: /
|   Total files found (by extension):
|_    
|_http-mobileversion-checker: No mobile version detected.
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
|_http-comments-displayer: Couldn't find any comments.
|_http-referer-checker: Couldn't find any cross-domain scripts.
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-date: Wed, 03 Apr 2024 04:01:25 GMT; -1s from local time.
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
| http-vhosts: 
| 16 names had status ERROR
|_112 names had status 404
|_http-title: Not Found
| http-headers: 
|   Content-Type: text/html; charset=us-ascii
|   Server: Microsoft-HTTPAPI/2.0
|   Date: Wed, 03 Apr 2024 04:01:29 GMT
|   Connection: close
|   Content-Length: 315
|   
|_  (Request type: GET)
|_http-malware-host: Host appears to be clean
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-feed: Couldn't find any feeds.
|_http-vuln-cve2014-3704: ERROR: Script execution failed (use -d to debug)
|_http-server-header: Microsoft-HTTPAPI/2.0
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:08:48 2024 -- 1 IP address (1 host up) scanned in 461.00 seconds
