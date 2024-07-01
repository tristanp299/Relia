# Nmap 7.94SVN scan initiated Tue Apr  2 21:08:10 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 47001 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/xml/tcp_47001_http_nmap.xml 192.168.224.247
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 21:08:10 PDT for 381s

Bug in http-security-headers: no string output.
PORT      STATE SERVICE REASON          VERSION
47001/tcp open  http    syn-ack ttl 125 Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-title: Not Found
|_http-feed: Couldn't find any feeds.
|_http-chrono: Request times for /; avg: 206.64ms; min: 204.40ms; max: 211.55ms
| http-useragent-tester: 
|   Status for browser useragent: 404
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
|     libcurl-agent/1.0
|     Python-urllib/2.5
|     GT::WWW
|     Snoopy
|     MFC_Tear_Sample
|     HTTP::Lite
|     URI::Fetch
|     Zend_Http_Client
|     http client
|_    Wget/1.13.4 (linux-gnu)
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
| http-headers: 
|   Content-Type: text/html; charset=us-ascii
|   Server: Microsoft-HTTPAPI/2.0
|   Date: Wed, 03 Apr 2024 04:08:32 GMT
|   Connection: close
|   Content-Length: 315
|   
|_  (Request type: GET)
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-comments-displayer: Couldn't find any comments.
|_http-mobileversion-checker: No mobile version detected.
|_http-referer-checker: Couldn't find any cross-domain scripts.
|_http-vuln-cve2014-3704: ERROR: Script execution failed (use -d to debug)
|_http-aspnet-debug: ERROR: Script execution failed (use -d to debug)
|_http-malware-host: Host appears to be clean
| http-vhosts: 
| 105 names had status 404
|_23 names had status ERROR
|_http-server-header: Microsoft-HTTPAPI/2.0
| http-errors: 
| Spidering limited to: maxpagecount=40; withinhost=192.168.224.247
|   Found the following error pages: 
|   
|   Error Code: 404
|_  	http://192.168.224.247:47001/
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-litespeed-sourcecode-download: Request with null byte did not work. This web server might not be vulnerable
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-date: Wed, 03 Apr 2024 04:08:32 GMT; 0s from local time.
| http-sitemap-generator: 
|   Directory structure:
|   Longest directory structure:
|     Depth: 0
|     Dir: /
|   Total files found (by extension):
|_    
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:14:31 2024 -- 1 IP address (1 host up) scanned in 381.32 seconds
