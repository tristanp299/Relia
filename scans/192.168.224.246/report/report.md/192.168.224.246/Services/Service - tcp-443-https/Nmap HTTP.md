```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 443 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/xml/tcp_443_https_nmap.xml" 192.168.224.246
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 21:01:03 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 443 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/xml/tcp_443_https_nmap.xml 192.168.224.246
Nmap scan report for 192.168.224.246
Host is up, received user-set (0.077s latency).
Scanned at 2024-04-02 21:01:03 PDT for 278s

PORT    STATE SERVICE  REASON         VERSION
443/tcp open  ssl/http syn-ack ttl 61 Apache httpd 2.4.52 ((Ubuntu))
| http-headers: 
|   Date: Wed, 03 Apr 2024 04:03:49 GMT
|   Server: Apache/2.4.52 (Ubuntu)
|   Vary: Accept-Encoding
|   Content-Length: 1516
|   Connection: close
|   Content-Type: text/html; charset=UTF-8
|   
|_  (Request type: GET)
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-csrf: Couldn't find any CSRF vulnerabilities.
| http-fileupload-exploiter: 
|   
|_    Couldn't find a file-type field.
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-chrono: Request times for /; avg: 536.13ms; min: 377.77ms; max: 1117.07ms
| http-errors: 
| Spidering limited to: maxpagecount=40; withinhost=192.168.224.246
|   Found the following error pages: 
|   
|   Error Code: 404
|_  	http://192.168.224.246:443/css/styles.css
|_http-malware-host: Host appears to be clean
|_http-feed: Couldn't find any feeds.
|_http-referer-checker: Couldn't find any cross-domain scripts.
|_http-mobileversion-checker: No mobile version detected.
|_http-traceroute: ERROR: Script execution failed (use -d to debug)
| ssl-cert: Subject: commonName=demo
| Subject Alternative Name: DNS:demo
| Issuer: commonName=demo
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2022-10-12T07:46:27
| Not valid after:  2032-10-09T07:46:27
| MD5:   6361:be08:5259:3a75:cd26:f869:1614:3c94
| SHA-1: 8fa0:04a7:5d03:4c29:44b7:6b14:119f:fd79:3c7e:5093
| -----BEGIN CERTIFICATE-----
| MIIC6TCCAdGgAwIBAgIUIN3Z/giwrWikVN/gzzofa98CJ1AwDQYJKoZIhvcNAQEL
| BQAwDzENMAsGA1UEAwwEZGVtbzAeFw0yMjEwMTIwNzQ2MjdaFw0zMjEwMDkwNzQ2
| MjdaMA8xDTALBgNVBAMMBGRlbW8wggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEK
| AoIBAQCMPw2+IkC55uip8gDmvy+mN/FtQJBck6audIht6POsdrE2GzfhAoxZY9al
| XkTc3WPOxP2X1I4ea1t1y8SQuX7jomUlNOgkGtVbj+RYzU8Qau7XWSTBMbVkRluc
| B+w5vPsGL1XGMd35V7Td6ZhotXLwc0j19smwewETujURfSmGCKdwbHztKozyW9Qg
| QFOtNI4gOHpvMxTYpR3QDkBYvIzaH+FaU8xqrr/GJiFSz8MUhxVPSM2QyqSmsFyE
| HYijIDbxBNRyf1lAmReLdwpwGqpRvBF1wYfpYyTvjW/j0LQPfvCcCVxD1v/3N3oK
| VR4/EYqBrCr9umF7Q3w5E4hC0x5VAgMBAAGjPTA7MAkGA1UdEwQCMAAwDwYDVR0R
| BAgwBoIEZGVtbzAdBgNVHQ4EFgQUqWpscb2cgQbMGE4Nh4vVDLAs55EwDQYJKoZI
| hvcNAQELBQADggEBACvVHEqW54LzwFNKfLMlbbrSitnXhGc1zgOaYdBnF95weO3j
| 5gEbGNElednFgWQEZzLz5ruS9i0aiKsQYKuh+AL+QQRdycfCbTxDVTopO9sxFYGd
| UpSxCGToYe5JULiNpnBpTWPEldc608y2jhpJpsH5UGifvRp/VpHW/3A+9t8oAUeN
| /SVW3bQ7sLEEvCmHH4E1uJS3k6kBidDY1A9OOxaL0k2v/cB8PONnEMwP4DcmKRA1
| cVrgXiR8x7E5zcVUPj8cM5+DqSOQTAphAcVbVx2c/K2XMENFZqVUbRFbuZSXVExp
| TQICNlWeutzCZGE7rREsIUUIigT9erEAvTu28RI=
|_-----END CERTIFICATE-----
|_ssl-date: TLS randomness does not represent time
| http-security-headers: 
|   Strict_Transport_Security: 
|_    HSTS not configured in HTTPS Server
| http-vhosts: 
|_128 names had status ERROR
|_http-userdir-enum: Potential Users: root, admin, administrator, webadmin, sysadmin, netadmin, guest, user, web, test
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-vuln-cve2014-3704: ERROR: Script execution failed (use -d to debug)
|_http-aspnet-debug: ERROR: Script execution failed (use -d to debug)
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1
|     /css/
|       css: 1
|     /icons/
|       gif: 3
|     /js/
|       Other: 1; js: 2
|   Longest directory structure:
|     Depth: 1
|     Dir: /js/
|   Total files found (by extension):
|_    Other: 2; css: 1; gif: 3; js: 2
|_http-title: 400 Bad Request
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
|     MFC_Tear_Sample
|     HTTP::Lite
|     PHPCrawl
|     URI::Fetch
|     http client
|     Wget/1.13.4 (linux-gnu)
|     WWW-Mechanize/1.34
|   Change in Status Code: 
|     Zend_Http_Client: 400
|     PECL::HTTP: 400
|_    Snoopy: 400
| ssl-enum-ciphers: 
|   TLSv1.3: 
|     ciphers: 
|       TLS_AKE_WITH_AES_128_GCM_SHA256 (ecdh_x25519) - A
|       TLS_AKE_WITH_AES_256_GCM_SHA384 (ecdh_x25519) - A
|       TLS_AKE_WITH_CHACHA20_POLY1305_SHA256 (ecdh_x25519) - A
|     cipher preference: client
|_  least strength: A
| http-sql-injection: 
|   Possible sqli for queries:
|     http://192.168.224.246:443/js/?C=S%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=M%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=D%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=N%3BO%3DD%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=S%3BO%3DD%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=N%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=M%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=D%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=S%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=N%3BO%3DA%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=M%3BO%3DD%27%20OR%20sqlspider
|     http://192.168.224.246:443/js/?C=D%3BO%3DA%27%20OR%20sqlspider
|_    http://192.168.224.246:443/js/?C=S%3BO%3DA%27%20OR%20sqlspider
| http-wordpress-enum: 
| Search limited to top 100 themes/plugins
|   themes
|_    twentyeleven
|_http-fetch: Please enter the complete path of the directory to save data in.
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.246
|     
|     Path: http://192.168.224.246:443/css/bootstrap.min.css
|     Line number: 1
|     Comment: 
|         /*!
|          * Bootstrap v3.3.7 (http://getbootstrap.com)
|          * Copyright 2011-2016 Twitter, Inc.
|          * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
|          */
|     
|     Path: http://192.168.224.246:443/
|     Line number: 14
|     Comment: 
|         <!-- <link rel="stylesheet" href="css/styles.css" /> -->
|     
|     Path: http://192.168.224.246:443/js/jquery-1.12.4.min.js
|     Line number: 1
|     Comment: 
|         /*! jQuery v1.12.4 | (c) jQuery Foundation | jquery.org/license */
|     
|     Path: http://192.168.224.246:443/css/bootstrap.min.css
|     Line number: 6
|     Comment: 
|         /*# sourceMappingURL=bootstrap.min.css.map */
|     
|     Path: http://192.168.224.246:443/css/bootstrap.min.css
|     Line number: 5
|     Comment: 
|         /*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
|     
|     Path: http://192.168.224.246:443/css/bootstrap.min.css
|     Line number: 5
|     Comment: 
|_        /*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
| http-grep: 
|   (1) https://192.168.224.246:443/css/styles.css: 
|     (1) ip: 
|_      + 192.168.224.246
|_http-server-header: Apache/2.4.52 (Ubuntu)

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:05:41 2024 -- 1 IP address (1 host up) scanned in 277.70 seconds

```
