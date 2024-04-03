# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:05 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp80/tcp_80_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp80/xml/tcp_80_http_nmap.xml 192.168.224.248
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.074s latency).
Scanned at 2024-04-02 20:58:06 PDT for 900s

PORT   STATE SERVICE REASON          VERSION
80/tcp open  http    syn-ack ttl 125 Microsoft IIS httpd 10.0
|_http-date: Wed, 03 Apr 2024 03:58:18 GMT; -2s from local time.
|_http-malware-host: Host appears to be clean
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
|_http-csrf: Couldn't find any CSRF vulnerabilities.
| http-headers: 
|   Cache-Control: no-cache
|   Pragma: no-cache
|   Content-Length: 22996
|   Content-Type: text/html; charset=utf-8
|   Expires: -1
|   Set-Cookie: dnn_IsMobile=False; path=/; HttpOnly
|   Set-Cookie: language=en-US; path=/; HttpOnly
|   Set-Cookie: .ASPXANONYMOUS=BMs0DXgdQd64dKooknGE-nNmcH3BTMeasHJ9CFL0VUrqxLs1_e2-l7rGQjDuysHXq2hFHb5fe-Pi8sieDLNZIqy4bZmbdGIuFgvQNbWo1yPsjYsR0; expires=Tue, 11-Jun-2024 14:38:15 GMT; path=/; HttpOnly
|   Set-Cookie: dnn_IsMobile=False; path=/; HttpOnly
|   Set-Cookie: language=en-US; path=/; HttpOnly
|   Set-Cookie: .ASPXANONYMOUS=BMs0DXgdQd64dKooknGE-nNmcH3BTMeasHJ9CFL0VUrqxLs1_e2-l7rGQjDuysHXq2hFHb5fe-Pi8sieDLNZIqy4bZmbdGIuFgvQNbWo1yPsjYsR0; expires=Tue, 11-Jun-2024 14:38:15 GMT; path=/; HttpOnly
|   X-UA-Compatible: IE=edge
|   Set-Cookie: dnn_IsMobile=False; path=/; HttpOnly
|   Set-Cookie: language=en-US; path=/; HttpOnly
|   Set-Cookie: .ASPXANONYMOUS=BMs0DXgdQd64dKooknGE-nNmcH3BTMeasHJ9CFL0VUrqxLs1_e2-l7rGQjDuysHXq2hFHb5fe-Pi8sieDLNZIqy4bZmbdGIuFgvQNbWo1yPsjYsR0; expires=Tue, 11-Jun-2024 14:38:15 GMT; path=/; HttpOnly
|   Set-Cookie: __RequestVerificationToken=82reQAaBPO2gvO_cYeiLwfrvnWMHCB4ADjANkkEU7Sc3gIJiDjn8Kzroppl1SsNQ7ht5pw2; path=/; HttpOnly
|   X-XSS-Protection: 1; mode=block
|   X-Frame-Options: SAMEORIGIN
|   Date: Wed, 03 Apr 2024 03:58:15 GMT
|   Connection: close
|   
|_  (Request type: HEAD)
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
| http-robots.txt: 16 disallowed entries 
| /*/ctl/ /admin/ /App_Browsers/ /App_Code/ /App_Data/ 
| /App_GlobalResources/ /bin/ /Components/ /Config/ /contest/ /controls/ 
| /Documentation/ /HttpModules/ /Install/ /Providers/ 
|_/Activity-Feed/userId/
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
| http-useragent-tester: 
|   Allowed User Agents: 
|     PHP/
|     HTTP::Lite
|     URI::Fetch
|   Change in Status Code: 
|     Wget/1.13.4 (linux-gnu): 200
|     http client: 200
|     GT::WWW: 200
|     libcurl-agent/1.0: 200
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html): 200
|     WWW-Mechanize/1.34: 200
|     lwp-trivial: 200
|     Zend_Http_Client: 200
|     MFC_Tear_Sample: 200
|     libwww: 200
|     PECL::HTTP: 200
|     Snoopy: 200
|     PHPCrawl: 200
|_    Python-urllib/2.5: 200
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
| http-vhosts: 
| 19 names had status ERROR
| 82 names had status 302
|_27 names had status 404
|_http-mobileversion-checker: No mobile version detected.
| http-php-version: Logo query returned unknown hash 9b9a4f16eb234052f80ba03da54bbe22
|_Credits query returned unknown hash d5ae02e2b7d3bf688c1a491ff14d9118
|_http-favicon: Unknown favicon MD5: 2DE6897008EB657D2EC770FE5B909439
|_http-litespeed-sourcecode-download: Request with null byte did not work. This web server might not be vulnerable
| http-security-headers: 
|   X_Frame_Options: 
|     Header: X-Frame-Options: SAMEORIGIN
|     Description: The browser must not display this content in any frame from a page of different origin than the content itself.
|   X_XSS_Protection: 
|     Header: X-XSS-Protection: 1; mode=block
|     Description: The browser will prevent the rendering of the page when XSS is detected.
|   Cache_Control: 
|     Header: Cache-Control: no-cache
|   Pragma: 
|     Header: Pragma: no-cache
|   Expires: 
|_    Header: Expires: -1
|_http-title: Home
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-devframework: ASP.NET detected. Found related header.
|_http-chrono: Request times for /; avg: 1965.69ms; min: 614.95ms; max: 6078.78ms
| http-unsafe-output-escaping: 
|   Characters [>] reflected in parameter returnurl at http://192.168.224.248:80/Login?returnurl=%2F
|   Characters [>] reflected in parameter returnurl at http://192.168.224.248:80/Login?returnurl=%2FTerms
|_  Characters [>] reflected in parameter returnurl at http://192.168.224.248:80/Login?returnurl=%2FPrivacy
| http-errors: 
| Spidering limited to: maxpagecount=40; withinhost=192.168.224.248
|   Found the following error pages: 
|   
|   Error Code: 404
|   	http://192.168.224.248:80/event.srcElement
|   
|   Error Code: 404
|_  	http://192.168.224.248:80/u;k=new
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.248
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 416
|     Comment: 
|         <!--CDF(Css|/Portals/_default/Skins/Xcillion/Menus/MainMenu/MainMenu.css?cdv=39|DnnPageHeaderProvider|14)-->
|     
|     Path: http://192.168.224.248:80/
|     Line number: 232
|     Comment: 
|         <!-- End_Module_355 -->
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 28
|     Comment: 
|         /* Chrome,Safari4+ */
|     
|     Path: http://192.168.224.248:80/ScriptResource.axd?d=Jw6tUGWnA15aQwrISj2e6KQ6kW_8KZV4DdhwRWF3O-0zvFgZ8W6sQJLaM92zdGSPG5whn8xyBSzcVLr6gNBePSSIaF-FKGTqx-IPnR7Asx8sNF7hGllZ9iOQ3XgQbrtyHpHaSvIIuKuESmMU0&amp;t=1156b909
|     Line number: 4
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 373
|     Comment: 
|         <!-- /.mainContent -->
|     
|     Path: http://192.168.224.248:80/WebResource.axd?d=pynGkmcFUV0PyGAbT-5Pql3C-BakzIWPan-7o6FF0Cg9AfDQUfO5XsBMkXU1&amp;t=637638679683537338
|     Line number: 105
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/js/dnncore.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 371
|     Comment: 
|         <!-- /.mainContent-inner -->
|     
|     Path: http://192.168.224.248:80/ScriptResource.axd?d=uHIkleVeDJcjSOnl0lixUQJRyqeLpMcg_bFKvurKVJGVqN4rcDGKCJjCwAnYaARt9BHBkbfOHs543B3sUAAP1IU4DDhIbZCtwf6LGO549QETw_fHaK66qNWmpLmpKXvSgZur1w2&amp;t=1156b909
|     Line number: 4
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.248:80/Resources/Search/
|     Line number: 219
|     Comment: 
|         <!-- Start_Module_362 -->
|     
|     Path: http://192.168.224.248:80/Resources/Search/
|     Line number: 52
|     Comment: 
|         
|         
|         <![endif]-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/js/dnn.js?cdv=39|DnnBodyProvider|12)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 216
|     Comment: 
|         <!-- Page Content -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Css|/Portals/0/home.css?cdv=39|DnnPageHeaderProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 60
|     Comment: 
|         <!-- UserControlPanel  -->
|     
|     Path: http://192.168.224.248:80/
|     Line number: 220
|     Comment: 
|         <!-- Start_Module_355 -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 271
|     Comment: 
|         /*globals jQuery, window, Sys */
|     
|     Path: http://192.168.224.248:80/ScriptResource.axd?d=uHIkleVeDJcjSOnl0lixUQJRyqeLpMcg_bFKvurKVJGVqN4rcDGKCJjCwAnYaARt9BHBkbfOHs543B3sUAAP1IU4DDhIbZCtwf6LGO549QETw_fHaK66qNWmpLmpKXvSgZur1w2&amp;t=1156b909
|     Line number: 2
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.248:80/WebResource.axd?d=pynGkmcFUV0PyGAbT-5Pql3C-BakzIWPan-7o6FF0Cg9AfDQUfO5XsBMkXU1&amp;t=637638679683537338
|     Line number: 85
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/Resources/libraries/jQuery/03_05_01/jquery.js?cdv=39|DnnPageHeaderProvider|5)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/Resources/Shared/Scripts/dnn.jquery.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/Resources/Shared/Scripts/jquery/jquery.hoverIntent.min.js?cdv=39|DnnBodyProvider|55)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Css|/Resources/Search/SearchSkinObjectPreview.css?cdv=39|DnnPageHeaderProvider|10)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 414
|     Comment: 
|         <!--CDF(Css|/Portals/_default/Skins/Xcillion/bootstrap/css/bootstrap.min.css?cdv=39|DnnPageHeaderProvider|12)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 375
|     Comment: 
|         <!-- /.container -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/js/dnn.servicesframework.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 417
|     Comment: 
|         <!--CDF(Css|/Portals/_default/Skins/Xcillion/skin.css?cdv=39|DnnPageHeaderProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 423
|     Comment: 
|         <!--CDF(Javascript|/Portals/_default/Skins/Xcillion/js/scripts.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Resources/Search/SearchSkinObjectPreview.js?cdv=39
|     Line number: 71
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 40
|     Comment: 
|         /* W3C */
|     
|     Path: http://192.168.224.248:80/WebResource.axd?d=pynGkmcFUV0PyGAbT-5Pql3C-BakzIWPan-7o6FF0Cg9AfDQUfO5XsBMkXU1&amp;t=637638679683537338
|     Line number: 100
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 377
|     Comment: 
|         <!-- Footer -->
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 34
|     Comment: 
|         /* Opera 11.10+ */
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 31
|     Comment: 
|         /* Chrome10+,Safari5.1+ */
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 25
|     Comment: 
|         /* FF3.6+ */
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 421
|     Comment: 
|         <!--CDF(Javascript|/Portals/_default/Skins/Xcillion/js/jquery.smartmenus.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 92
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 53
|     Comment: 
|         
|         
|         
|         <![endif]-->
|     
|     Path: http://192.168.224.248:80/
|     Line number: 325
|     Comment: 
|         <!-- End_Module_354 -->
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 1
|     Comment: 
|         /* Home Page style */
|     
|     Path: http://192.168.224.248:80/Resources/Search/
|     Line number: 226
|     Comment: 
|         <!-- End_Module_362 -->
|     
|     Path: http://192.168.224.248:80/
|     Line number: 237
|     Comment: 
|         <!-- Start_Module_354 -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Css|/Resources/Shared/stylesheets/dnndefault/7.0.0/default.css?cdv=39|DnnPageHeaderProvider|5)-->
|     
|     Path: http://192.168.224.248:80/Portals/0/home.css?cdv=39
|     Line number: 37
|     Comment: 
|         /* IE10+ */
|     
|     Path: http://192.168.224.248:80/Resources/Search/SearchSkinObjectPreview.js?cdv=39
|     Line number: 85
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 415
|     Comment: 
|         <!--CDF(Css|/Portals/_default/Skins/Xcillion/css/jquery.smartmenus.bootstrap.css?cdv=39|DnnPageHeaderProvider|13)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 420
|     Comment: 
|         <!--CDF(Javascript|/Portals/_default/Skins/Xcillion/bootstrap/js/bootstrap.min.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Resources/Search/SearchSkinObjectPreview.js?cdv=39
|     Line number: 94
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Css|/DesktopModules/Admin/Authentication/module.css?cdv=39|DnnPageHeaderProvider|10)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/Resources/libraries/jQuery-UI/01_13_02/jquery-ui.min.js?cdv=39|DnnPageHeaderProvider|10)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/Resources/Search/SearchSkinObjectPreview.js?cdv=39|DnnBodyProvider|100)-->
|     
|     Path: http://192.168.224.248:80/Resources/Search/SearchSkinObjectPreview.js?cdv=39
|     Line number: 69
|     Comment: 
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 28
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 176
|     Comment: 
|         <!--Header -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 166
|     Comment: 
|         /*showReturn*/
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/Resources/libraries/jQuery-Migrate/03_04_00/jquery-migrate.js?cdv=39|DnnPageHeaderProvider|6)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Css|/Portals/_default/Skins/Xcillion/skin.css?cdv=39|DnnPageHeaderProvider|15)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 435
|     Comment: 
|         <!--CDF(Javascript|/js/dnn.modalpopup.js?cdv=39|DnnBodyProvider|50)-->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 16
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 188
|     Comment: 
|         <!-- Brand and toggle get grouped for better mobile display -->
|     
|     Path: http://192.168.224.248:80/event.srcElement
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
|         -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 411
|     Comment: 
|         <!-- /.SiteWrapper -->
|     
|     Path: http://192.168.224.248:80/Login?returnurl=%2FPrivacy
|     Line number: 422
|     Comment: 
|_        <!--CDF(Javascript|/Portals/_default/Skins/Xcillion/js/jquery.smartmenus.bootstrap.js?cdv=39|DnnBodyProvider|100)-->
| http-auth-finder: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.248
|   url                                                   method
|   http://192.168.224.248:80/Login?returnurl=%2F         FORM
|   http://192.168.224.248:80/Login?returnurl=%2FTerms    FORM
|_  http://192.168.224.248:80/Login?returnurl=%2FPrivacy  FORM
| http-grep: 
|   (1) http://192.168.224.248:80/: 
|     (1) ip: 
|       + 192.168.224.248
|   (1) http://192.168.224.248:80/Terms: 
|     (1) email: 
|_      + emma@relia.com
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 4; axd: 2
|     /Portals/0/
|       css: 1
|     /Portals/0/Images/
|       png: 1
|     /Resources/Search/
|       css: 1; js: 1
|     /js/
|       js: 4
|     /portals/0/Images/
|       png: 1
|   Longest directory structure:
|     Depth: 3
|     Dir: /portals/0/Images/
|   Total files found (by extension):
|_    Other: 4; axd: 2; css: 2; js: 5; png: 2
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-feed: Couldn't find any feeds.
| http-fileupload-exploiter: 
|   
|_    Couldn't find a file-type field.
| http-referer-checker: 
| Spidering limited to: maxpagecount=30
|   https://oss.maxcdn.com:443/respond/1.4.2/respond.min.js
|_  https://cdnjs.cloudflare.com:443/ajax/libs/html5shiv/3.7.2/html5shiv.min.js
| http-enum: 
|   /login.aspx: Possible admin folder
|   /rss.aspx: RSS or Atom feed
|   /login/: Login page
|   /robots.txt: Robots file
|_  /privacy/: Potentially interesting folder
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:13:06 2024 -- 1 IP address (1 host up) scanned in 900.74 seconds
