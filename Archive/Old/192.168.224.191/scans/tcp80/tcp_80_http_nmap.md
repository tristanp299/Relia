# Nmap 7.94SVN scan initiated Tue Apr  2 21:04:53 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.191/scans/tcp80/tcp_80_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.191/scans/tcp80/xml/tcp_80_http_nmap.xml 192.168.224.191
Nmap scan report for 192.168.224.191
Host is up, received user-set (0.082s latency).
Scanned at 2024-04-02 21:04:53 PDT for 251s

Bug in http-security-headers: no string output.
PORT   STATE SERVICE REASON          VERSION
80/tcp open  http    syn-ack ttl 125 Microsoft IIS httpd 10.0
|_http-comments-displayer: Couldn't find any comments.
|_http-chrono: Request times for /; avg: 509.61ms; min: 212.17ms; max: 1268.24ms
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-date: Wed, 03 Apr 2024 04:05:20 GMT; -2s from local time.
| http-errors: 
| Spidering limited to: maxpagecount=40; withinhost=192.168.224.191
|   Found the following error pages: 
|   
|   Error Code: 400
|_  	http://192.168.224.191:80/
|_http-referer-checker: Couldn't find any cross-domain scripts.
| http-vhosts: 
| 101 names had status 401
|_27 names had status ERROR
|_http-aspnet-debug: ERROR: Script execution failed (use -d to debug)
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-userdir-enum: Potential Users: root, admin, administrator, webadmin, sysadmin, netadmin, guest, user, web, test
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-title: Bad Request
|_http-malware-host: Host appears to be clean
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
|_http-fetch: Please enter the complete path of the directory to save data in.
| http-sitemap-generator: 
|   Directory structure:
|   Longest directory structure:
|     Depth: 0
|     Dir: /
|   Total files found (by extension):
|_    
| http-useragent-tester: 
|   Status for browser useragent: 401
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
|     libcurl-agent/1.0
|     PHP/
|     Python-urllib/2.5
|     GT::WWW
|     MFC_Tear_Sample
|     HTTP::Lite
|     PHPCrawl
|     URI::Fetch
|     Zend_Http_Client
|     http client
|     PECL::HTTP
|     Wget/1.13.4 (linux-gnu)
|_    WWW-Mechanize/1.34
|_http-feed: Couldn't find any feeds.
| http-auth: 
| HTTP/1.1 401 Unauthorized\x0D
|_  Basic realm=192.168.224.191
|_http-server-header: Microsoft-IIS/10.0
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
|_http-litespeed-sourcecode-download: Request with null byte did not work. This web server might not be vulnerable
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-mobileversion-checker: No mobile version detected.
|_http-vuln-cve2014-3704: ERROR: Script execution failed (use -d to debug)
| http-headers: 
|   Content-Type: text/html; charset=us-ascii
|   Server: Microsoft-HTTPAPI/2.0
|   Date: Wed, 03 Apr 2024 04:05:20 GMT
|   Connection: close
|   Content-Length: 339
|   
|_  (Request type: GET)
| http-wordpress-enum: 
| Search limited to top 100 themes/plugins
|   plugins
|     akismet
|     contact-form-7
|     wordpress-seo
|     jetpack
|     all-in-one-seo-pack
|     wordfence
|     woocommerce
|     google-sitemap-generator
|     wordpress-importer
|     nextgen-gallery
|     google-analytics-for-wordpress
|     wp-super-cache
|     tinymce-advanced
|     wptouch
|     better-wp-security
|     siteorigin-panels
|     updraftplus
|     w3-total-cache
|     google-analytics-dashboard-for-wp
|     wp-pagenavi
|     si-contact-form
|     advanced-custom-fields
|     mailchimp-for-wp
|     the-events-calendar
|     add-to-any
|     duplicator
|     wysija-newsletters
|     ninja-forms
|     wp-smushit
|     buddypress
|     ewww-image-optimizer
|     so-widgets-bundle
|     really-simple-captcha
|     ml-slider
|     black-studio-tinymce-widget
|     photo-gallery
|     broken-link-checker
|     regenerate-thumbnails
|     google-analyticator
|     redirection
|     captcha
|     duplicate-post
|     breadcrumb-navxt
|     backwpup
|     user-role-editor
|     yet-another-related-posts-plugin
|     contact-form-plugin
|     newsletter
|     bbpress
|     all-in-one-wp-security-and-firewall
|     disable-comments
|     social-networks-auto-poster-facebook-twitter-g
|     wp-optimize
|     addthis
|     wp-statistics
|     wp-e-commerce
|     all-in-one-wp-migration
|     backupwordpress
|     si-captcha-for-wordpress
|     wp-slimstat
|     wp-google-maps
|     wp-spamshield
|     wp-maintenance-mode
|     googleanalytics
|     worker
|     yith-woocommerce-wishlist
|     wp-multibyte-patch
|     wp-to-twitter
|     image-widget
|     wp-db-backup
|     shortcodes-ultimate
|     ultimate-tinymce
|     share-this
|     disqus-comment-system
|     gallery-bank
|     types
|     wp-polls
|     custom-post-type-ui
|     shareaholic
|     polylang
|     post-types-order
|     gtranslate
|     bulletproof-security
|     wp-fastest-cache
|     facebook
|     sociable
|     iwp-client
|     nextgen-facebook
|     seo-ultimate
|     wp-postviews
|     formidable
|     squirrly-seo
|     wp-mail-smtp
|     tablepress
|     redux-framework
|     page-links-to
|     youtube-embed-plus
|     contact-bank
|     maintenance
|     wp-retina-2x
|   themes
|     twentyeleven
|     twentytwelve
|     twentyten
|     twentythirteen
|     twentyfourteen
|     twentyfifteen
|     responsive
|     customizr
|     zerif-lite
|     virtue
|     storefront
|     atahualpa
|     twentysixteen
|     vantage
|     hueman
|     spacious
|     evolve
|     colorway
|     graphene
|     sydney
|     ifeature
|     mh-magazine-lite
|     generatepress
|     mantra
|     omega
|     onetone
|     coraline
|     pinboard
|     thematic
|     sparkling
|     catch-box
|     make
|     colormag
|     enigma
|     custom-community
|     mystique
|     alexandria
|     delicate
|     lightword
|     attitude
|     inove
|     magazine-basic
|     raindrops
|     minamaze
|     zbench
|     point
|     eclipse
|     portfolio-press
|     twentyseventeen
|     travelify
|     swift-basic
|     iconic-one
|     arcade-basic
|     bouquet
|     pixel
|     sliding-door
|     pilcrow
|     simple-catch
|     tempera
|     destro
|     p2
|     sunspot
|     sundance
|     dusk-to-dawn
|     onepress
|     moesia
|     dynamic-news-lite
|     parabola
|     parament
|     dazzling
|     accesspress-lite
|     optimizer
|     one-page
|     chaostheory
|     business-lite
|     duster
|     constructor
|     nirvana
|     sixteen
|     esquire
|     beach
|     next-saturday
|     flat
|     hatch
|     minimatica
|     radiate
|     accelerate
|     oxygen
|     accesspress-parallax
|     swift
|     spun
|     wp-creativix
|     suevafree
|     hemingway
|     pink-touch-2
|     motion
|     fruitful
|     steira
|     news
|_    llorix-one-lite
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:09:04 2024 -- 1 IP address (1 host up) scanned in 251.41 seconds
