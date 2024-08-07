# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:10 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/xml/tcp_80_http_nmap.xml 192.168.224.247
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.075s latency).
Scanned at 2024-04-02 20:58:10 PDT for 515s

Bug in http-security-headers: no string output.
PORT   STATE SERVICE REASON          VERSION
80/tcp open  http    syn-ack ttl 125 Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
| http-trace: TRACE is enabled
| Headers:
| Date: Wed, 03 Apr 2024 03:58:19 GMT
| Server: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
| Connection: close
| Transfer-Encoding: chunked
|_Content-Type: message/http
|_http-errors: Couldn't find any error pages.
|_http-feed: Couldn't find any feeds.
|_http-title: RELIA - New Hire Information
|_http-malware-host: Host appears to be clean
|_http-aspnet-debug: ERROR: Script execution failed (use -d to debug)
| http-php-version: Credits query returned unknown hash 443ee98ec8f6fb0eb7e56948348e0f32
|_Version from header x-powered-by: PHP/8.1.10
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1
|     /css/
|       css: 1
|     /js/
|       js: 1
|     /pdfs/
|       pdf: 2
|   Longest directory structure:
|     Depth: 1
|     Dir: /pdfs/
|   Total files found (by extension):
|_    Other: 1; css: 1; js: 1; pdf: 2
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
| http-vhosts: 
| 46 names had status 200
|_82 names had status ERROR
|_http-referer-checker: Couldn't find any cross-domain scripts.
|_http-csrf: Couldn't find any CSRF vulnerabilities.
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.247
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 16
|     Comment: 
|          // if (localStorage.getItem('sb|sidebar-toggle') === 'true') {
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 6117
|     Comment: 
|         /* rtl:options: {
|           "autoRename": true,
|           "stringMap":[ {
|             "name"    : "prev-next",
|             "search"  : "prev",
|             "replace" : "next"
|           } ]
|         } */
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 12
|     Comment: 
|          // Toggle the side navigation
|     
|     Path: http://192.168.224.247:80/
|     Line number: 13
|     Comment: 
|         <!-- Sidebar-->
|     
|     Path: http://192.168.224.247:80/
|     Line number: 21
|     Comment: 
|         <!-- <a class="list-group-item list-group-item-action list-group-item-light p-3" href="#!">Laptop and Mobile Phone</a> -->
|     
|     Path: http://192.168.224.247:80/
|     Line number: 25
|     Comment: 
|         <!-- Page content wrapper-->
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 7
|     Comment: 
|         /*!
|          * Bootstrap v5.1.3 (https://getbootstrap.com/)
|          * Copyright 2011-2021 The Bootstrap Authors
|          * Copyright 2011-2021 Twitter, Inc.
|          * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
|          */
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 6
|     Comment: 
|         
|         // 
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 15
|     Comment: 
|          // Uncomment Below to persist sidebar toggle between refreshes
|     
|     Path: http://192.168.224.247:80/
|     Line number: 22
|     Comment: 
|         <!-- <a class="list-group-item list-group-item-action list-group-item-light p-3" href="#!">A word from the CEO</a> -->
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 18
|     Comment: 
|          // }
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 17
|     Comment: 
|          //     document.body.classList.toggle('sb-sidenav-toggled');
|     
|     Path: http://192.168.224.247:80/
|     Line number: 27
|     Comment: 
|         <!-- Top navigation-->
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 7716
|     Comment: 
|         /* rtl:end:remove */
|     
|     Path: http://192.168.224.247:80/
|     Line number: 20
|     Comment: 
|         <!-- <a class="list-group-item list-group-item-action list-group-item-light p-3" href="/pdfs/New-Hire-Form.pdf">New Hire Form</a> -->
|     
|     Path: http://192.168.224.247:80/
|     Line number: 40
|     Comment: 
|         <!-- Page content-->
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 7710
|     Comment: 
|         /* rtl:begin:remove */
|     
|     Path: http://192.168.224.247:80/js/scripts.js
|     Line number: 1
|     Comment: 
|         /*!
|         * Start Bootstrap - Simple Sidebar v6.0.5 (https://startbootstrap.com/template/simple-sidebar)
|         * Copyright 2013-2022 Start Bootstrap
|         * Licensed under MIT (https://github.com/StartBootstrap/startbootstrap-simple-sidebar/blob/master/LICENSE)
|         */
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 4791
|     Comment: 
|         /* rtl: var(--bs-breadcrumb-divider, "/") */
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 256
|     Comment: 
|         /* rtl:ignore */
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 6041
|     Comment: 
|         /* rtl:end:ignore */
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 440
|     Comment: 
|         /* rtl:raw:
|         [type="tel"],
|         [type="url"],
|         [type="email"],
|         [type="number"] {
|           direction: ltr;
|         }
|         */
|     
|     Path: http://192.168.224.247:80/css/styles.css
|     Line number: 6030
|     Comment: 
|_        /* rtl:begin:ignore */
|_http-vuln-cve2014-3704: ERROR: Script execution failed (use -d to debug)
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-date: Wed, 03 Apr 2024 03:58:26 GMT; 0s from local time.
|_http-chrono: Request times for /; avg: 10593.41ms; min: 1607.67ms; max: 22218.82ms
|_http-mobileversion-checker: No mobile version detected.
| http-useragent-tester: 
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     lwp-trivial
|     libcurl-agent/1.0
|     PHP/
|     HTTP::Lite
|     PHPCrawl
|     http client
|     PECL::HTTP
|     Wget/1.13.4 (linux-gnu)
|     WWW-Mechanize/1.34
|   Change in Status Code: 
|     MFC_Tear_Sample: 200
|     Zend_Http_Client: 200
|     Python-urllib/2.5: 200
|     Snoopy: 200
|     libwww: 200
|     GT::WWW: 200
|_    URI::Fetch: 200
| http-headers: 
|   Date: Wed, 03 Apr 2024 03:58:47 GMT
|   Server: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
|   X-Powered-By: PHP/8.1.10
|   Connection: close
|   Content-Type: text/html; charset=UTF-8
|   
|_  (Request type: HEAD)
| http-methods: 
|_  Supported Methods: GET
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:06:45 2024 -- 1 IP address (1 host up) scanned in 515.96 seconds
