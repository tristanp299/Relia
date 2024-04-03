```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 8000 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/xml/tcp_8000_http_nmap.xml" 192.168.224.245
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:59:33 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 8000 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/xml/tcp_8000_http_nmap.xml 192.168.224.245
Nmap scan report for 192.168.224.245
Host is up, received user-set (0.076s latency).
Scanned at 2024-04-02 20:59:33 PDT for 63s

Bug in http-security-headers: no string output.
PORT     STATE SERVICE REASON         VERSION
8000/tcp open  http    syn-ack ttl 61 Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
| http-headers: 
|   Date: Wed, 03 Apr 2024 04:00:04 GMT
|   Server: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
|   Last-Modified: Wed, 12 Oct 2022 08:56:01 GMT
|   ETag: "6ad-5ead28fdcdb81"
|   Accept-Ranges: bytes
|   Content-Length: 1709
|   Connection: close
|   Content-Type: text/html
|   
|_  (Request type: HEAD)
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1
|     /img/
|       png: 1
|     /js/
|       js: 1
|     /style/
|       css: 1
|   Longest directory structure:
|     Depth: 1
|     Dir: /js/
|   Total files found (by extension):
|_    Other: 1; css: 1; js: 1; png: 1
|_http-feed: Couldn't find any feeds.
|_http-litespeed-sourcecode-download: Request with null byte did not work. This web server might not be vulnerable
|_http-php-version: Logo query returned unknown hash 91c0ad4eec140f8fb514f335383d477c
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
|_http-date: Wed, 03 Apr 2024 03:59:56 GMT; -1s from local time.
|_http-referer-checker: Couldn't find any cross-domain scripts.
| http-useragent-tester: 
|   Status for browser useragent: 200
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
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
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-chrono: Request times for /; avg: 1655.86ms; min: 206.43ms; max: 4319.68ms
|_http-errors: Couldn't find any error pages.
| http-vhosts: 
| 90 names had status 200
|_38 names had status ERROR
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-title: Site doesn't have a title (text/html).
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-malware-host: Host appears to be clean
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
| http-csrf: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.245
|   Found the following possible CSRF vulnerabilities: 
|     
|     Path: http://192.168.224.245:8000/
|     Form id: username
|_    Form action: javascript:doLogin()
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
| http-auth-finder: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.245
|   url                           method
|_  http://192.168.224.245:8000/  FORM
| http-enum: 
|_  /login/: Login page
|_http-mobileversion-checker: No mobile version detected.
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.245
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 98
|     Comment: 
|         /*style the close button*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 69
|     Comment: 
|         /*set the forgot password text*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 90
|     Comment: 
|         /*style the model content box*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 64
|     Comment: 
|         /*set padding to the container*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 46
|     Comment: 
|         /*set extra style for the cancel button*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 53
|     Comment: 
|         /*centre the display image inside the container*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 20
|     Comment: 
|         /*assign full width inputs*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 75
|     Comment: 
|         /*set the Modal background*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 114
|     Comment: 
|         /* add zoom animation*/
|     
|     Path: http://192.168.224.245:8000/style/style.css
|     Line number: 41
|     Comment: 
|_        /* set a hover effect for the button*/

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:00:36 2024 -- 1 IP address (1 host up) scanned in 63.62 seconds

```
