```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/xml/tcp_80_http_nmap.xml" 192.168.224.245
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:55 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/xml/tcp_80_http_nmap.xml 192.168.224.245
Nmap scan report for 192.168.224.245
Host is up, received user-set (0.10s latency).
Scanned at 2024-04-02 20:58:55 PDT for 150s

Bug in http-security-headers: no string output.
PORT   STATE SERVICE REASON         VERSION
80/tcp open  http    syn-ack ttl 61 Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-php-version: Logo query returned unknown hash 28760c5364129774709f925bb8804012
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
| http-headers: 
|   Date: Wed, 03 Apr 2024 03:59:26 GMT
|   Server: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
|   Last-Modified: Wed, 12 Oct 2022 08:56:01 GMT
|   ETag: "b4b6-5ead28fde71bf"
|   Accept-Ranges: bytes
|   Content-Length: 46262
|   Connection: close
|   Content-Type: text/html
|   
|_  (Request type: HEAD)
|_http-mobileversion-checker: No mobile version detected.
|_http-feed: Couldn't find any feeds.
|_http-litespeed-sourcecode-download: Request with null byte did not work. This web server might not be vulnerable
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-date: Wed, 03 Apr 2024 03:59:26 GMT; -1s from local time.
|_http-aspnet-debug: ERROR: Script execution failed (use -d to debug)
|_http-malware-host: Host appears to be clean
|_http-fetch: Please enter the complete path of the directory to save data in.
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1
|     /bootstrap/js/
|       js: 1
|     /css/
|       css: 1
|     /css/colors/
|       css: 1
|     /css/font-awesome/css/
|       css: 1
|     /img/assets/
|       png: 1
|     /img/backgrounds/
|       jpg: 1
|     /img/clients/
|       png: 6
|     /img/team/
|       png: 1
|     /js/plugins/
|       js: 6
|   Longest directory structure:
|     Depth: 3
|     Dir: /css/font-awesome/css/
|   Total files found (by extension):
|_    Other: 1; css: 3; jpg: 1; js: 7; png: 8
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-errors: Couldn't find any error pages.
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
|_http-exif-spider: ERROR: Script execution failed (use -d to debug)
| http-grep: 
|   (1) http://192.168.224.245:80/js/plugins/tweetie.min.js: 
|     (1) email: 
|       + hi@sonnyt.com
|   (1) http://192.168.224.245:80/js/plugins/revslider.min.js: 
|     (1) email: 
|       + jack@greensock.com
|   (1) http://192.168.224.245:80/js/plugins/gmap3.min.js: 
|     (1) email: 
|       + jbdemonte@gmail.com
|   (1) http://192.168.224.245:80/js/plugins/smoothscroll.min.js: 
|     (1) email: 
|_      + patrickb1991@gmail.com
| http-comments-displayer: 
| Spidering limited to: maxdepth=3; maxpagecount=20; withinhost=192.168.224.245
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2358
|     Comment: 
|         /* Form style */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 3402
|     Comment: 
|         /*----- Blog -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2886
|     Comment: 
|         /*-- Buttons --*/
|     
|     Path: http://192.168.224.245:80/bootstrap/css/bootstrap.min.css
|     Line number: 6
|     Comment: 
|         /*# sourceMappingURL=bootstrap.min.css.map */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 2
|     Comment: 
|         
|         
|         
|         
|         -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2280
|     Comment: 
|         /*----- Testimonials -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2852
|     Comment: 
|         /*----- Back to Top Button -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 9
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
|         ------------------------------------------------------------------------------*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2497
|     Comment: 
|         /*----- Google maps -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2594
|     Comment: 
|         /*----- Footer 1 -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 290
|     Comment: 
|         <!-- End Home Revolution Slider Parallax Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 498
|     Comment: 
|         /*----- Home Sections -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 715
|     Comment: 
|         /*----- Home Revolution Slider -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 842
|     Comment: 
|         <!-- End Footer Widgets -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 911
|     Comment: 
|         <!-- End Footer 1 -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1105
|     Comment: 
|         /* End Logo Big White */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 69
|     Comment: 
|         <!-- Collect the nav links, forms, and other content for toggling -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1630
|     Comment: 
|         /*----- Quote -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 710
|     Comment: 
|         <!-- End Services Section -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 294
|     Comment: 
|         <!-- Start Features Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2803
|     Comment: 
|         /*---- Home Landing Subscribe Form -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 104
|     Comment: 
|         <!-- End Header -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 913
|     Comment: 
|         <!-- Start Back To Top -->
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 47
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
|          */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 49
|     Comment: 
|         <!-- End Preloader -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 53
|     Comment: 
|         /*----- General ----*/
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 133
|     Comment: 
|         
|          */
|     
|     Path: http://192.168.224.245:80/js/plugins/tweetie.min.js
|     Line number: 1
|     Comment: 
|         
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 37
|     Comment: 
|         
|            its values is > 50%. */
|     
|     Path: http://192.168.224.245:80/js/plugins/moderniz.min.js
|     Line number: 1
|     Comment: 
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/bootstrap/css/bootstrap.min.css
|     Line number: 5
|     Comment: 
|         /*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
|     
|     Path: http://192.168.224.245:80/css/colors/green.css
|     Line number: 1
|     Comment: 
|         
|         
|         
|         
|         */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1106
|     Comment: 
|         /* Logo Small Black */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 3311
|     Comment: 
|         /*----- Owl Carousel -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1491
|     Comment: 
|         /* Img Hover Effect */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2503
|     Comment: 
|         /*----- Video Popup Section -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 778
|     Comment: 
|         <!-- Start Testimonials Section -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 17
|     Comment: 
|         <!-- Stlylesheet -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 3247
|     Comment: 
|         /*--tabs--*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2063
|     Comment: 
|         /*----- Price List -----*/
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 144
|     Comment: 
|         
|         
|         
|         
|         
|         **************************************************************************/
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 2
|     Comment: 
|         
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 789
|     Comment: 
|         /*----- Header -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 222
|     Comment: 
|         <!-- SLIDE 3 -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 966
|     Comment: 
|         /*Navbar Collapse*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 406
|     Comment: 
|         <!-- End About Section -->
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 110
|     Comment: 
|         
|          */
|     
|     Path: http://192.168.224.245:80/js/plugins/easign1.3.min.js
|     Line number: 1
|     Comment: 
|         
|         
|         */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 214
|     Comment: 
|         /* Preloader */
|     
|     Path: http://192.168.224.245:80/css/font-awesome/css/font-awesome.css
|     Line number: 169
|     Comment: 
|         
|            readers do not read off random characters that represent icons */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 762
|     Comment: 
|         <!-- Start Call to Action 1 -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1590
|     Comment: 
|         /*----- Fun Facts -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 445
|     Comment: 
|         <!-- Start Team Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1130
|     Comment: 
|         /* End Logo Small Black */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1973
|     Comment: 
|         /*----- Get Connected -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1284
|     Comment: 
|         /*----- Features -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 3328
|     Comment: 
|         /* Applies a "closed-hand" cursor during drag operation. */
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 73
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
|          **/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 99
|     Comment: 
|         <!-- /.navbar-collapse -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 55
|     Comment: 
|         <!-- Brand and toggle get grouped for better mobile display -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 106
|     Comment: 
|         <!-- Start Home Revolution Slider Parallax Section -->
|     
|     Path: http://192.168.224.245:80/js/plugins/cubeportfolio.min.js
|     Line number: 1
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
|          */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1961
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
|         */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 146
|     Comment: 
|         <!-- Home Button -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 776
|     Comment: 
|         <!-- End Call to Action 1 -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 910
|     Comment: 
|         /*Navbar Toggle*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 47
|     Comment: 
|         /*----- Fonts -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 10
|     Comment: 
|         <!-- Meta Data -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 594
|     Comment: 
|         <!-- Start Quote Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1447
|     Comment: 
|         /*----- Team -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1704
|     Comment: 
|         /*----- Portfolio -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 818
|     Comment: 
|         /*border-bottom: 1px solid rgba(255,255,255,0.25);*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 920
|     Comment: 
|         <!-- End Site Wrapper -->
|     
|     Path: http://192.168.224.245:80/bootstrap/js/bootstrap.min.js
|     Line number: 1
|     Comment: 
|         
|         
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/js/plugins/owlcarousel.min.js
|     Line number: 1
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
|          */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1390
|     Comment: 
|         /*----- Skills -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 629
|     Comment: 
|         <!-- End Quote Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1075
|     Comment: 
|         /* Logo Big White */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 631
|     Comment: 
|         <!-- Start Portfolio Section -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 116
|     Comment: 
|         <!-- Home Heading -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 112
|     Comment: 
|         <!-- SLIDE 1 -->
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 60
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
|          */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2041
|     Comment: 
|         /*----- Services -----*/
|     
|     Path: http://192.168.224.245:80/js/plugins/counterup.min.js
|     Line number: 1
|     Comment: 
|         
|         
|         
|         
|         
|         
|         
|         */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2843
|     Comment: 
|         /*----- Twitter Feed -----*/
|     
|     Path: http://192.168.224.245:80/bootstrap/css/bootstrap.min.css
|     Line number: 5
|     Comment: 
|         /*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
|     
|     Path: http://192.168.224.245:80/bootstrap/css/bootstrap.min.css
|     Line number: 1
|     Comment: 
|         
|         
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1677
|     Comment: 
|         /* IE 9 */
|     
|     Path: http://192.168.224.245:80/css/font-awesome/css/font-awesome.css
|     Line number: 1
|     Comment: 
|         
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/js/plugins/parallax.min.js
|     Line number: 1
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
|         */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 28
|     Comment: 
|         <!-- Start Preloader -->
|     
|     Path: http://192.168.224.245:80/js/no-ui-slider/jquery.nouislider.all.min.js
|     Line number: 1
|     Comment: 
|         /*! noUiSlider - 7.0.10 - 2014-12-27 14:50:47 */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2337
|     Comment: 
|         /*----- Contact Form -----*/
|     
|     Path: http://192.168.224.245:80/js/plugins/smoothscroll.min.js
|     Line number: 6
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.245:80/
|     Line number: 23
|     Comment: 
|         <!-- Skin Color -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1140
|     Comment: 
|         /*Dropdown*/
|     
|     Path: http://192.168.224.245:80/js/plugins/smoothscroll.min.js
|     Line number: 2
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.245:80/
|     Line number: 51
|     Comment: 
|         <!-- Start Header -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 838
|     Comment: 
|         <!-- End Testimonials Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2884
|     Comment: 
|         /*----- Shortcodes -----*/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2230
|     Comment: 
|         /*----- Clients -----*/
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 42
|     Comment: 
|         
|            creates a new context for the origins. */
|     
|     Path: http://192.168.224.245:80/js/plugins/waypoints.min.js
|     Line number: 2
|     Comment: 
|         
|         
|         
|         
|         
|         */
|     
|     Path: http://192.168.224.245:80/js/plugins/jquery.min.js
|     Line number: 1
|     Comment: 
|         /*! jQuery v1.11.3 | (c) 2005, 2015 jQuery Foundation, Inc. | jquery.org/license */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 167
|     Comment: 
|         <!-- SLIDE 2 -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 712
|     Comment: 
|         <!-- Start Clients Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 1361
|     Comment: 
|         /*----- About Section -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 908
|     Comment: 
|         <!-- End Footer Copyright -->
|     
|     Path: http://192.168.224.245:80/js/plugins/smoothscroll.min.js
|     Line number: 4
|     Comment: 
|         
|         
|     
|     Path: http://192.168.224.245:80/
|     Line number: 921
|     Comment: 
|         <!-- jQuery -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 131
|     Comment: 
|         <!-- Home Subheading -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 101
|     Comment: 
|         <!-- /.container -->
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 8
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
|         */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 840
|     Comment: 
|         <!-- Start Footer 1 -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 367
|     Comment: 
|         <!--End Features Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2053
|     Comment: 
|         /*----- Call To Action 1 -----*/
|     
|     Path: http://192.168.224.245:80/css/font-awesome/css/font-awesome.css
|     Line number: 5
|     Comment: 
|         
|          * -------------------------- */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 592
|     Comment: 
|         <!-- End Team Section -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 643
|     Comment: 
|         <!-- Start Get Connected -->
|     
|     Path: http://192.168.224.245:80/
|     Line number: 760
|     Comment: 
|         <!-- End Clients Section -->
|     
|     Path: http://192.168.224.245:80/js/plugins/gmap3.min.js
|     Line number: 1
|     Comment: 
|         
|         
|         
|         
|         
|         
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 62
|     Comment: 
|         
|          */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 408
|     Comment: 
|         <!-- Start Fun Facts Section -->
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 83
|     Comment: 
|         
|          */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 443
|     Comment: 
|         <!-- End Fun Facts Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 41
|     Comment: 
|         /*----- Stylesheets -----*/
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 54
|     Comment: 
|         
|         
|          */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 641
|     Comment: 
|         <!-- End Portfolio Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 742
|     Comment: 
|         /*-webkit-transition: 1s opacity ease-in-out;*/
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 100
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
|          */
|     
|     Path: http://192.168.224.245:80/css/no-ui-slider/jquery.nouislider.css
|     Line number: 160
|     Comment: 
|         
|          */
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 2697
|     Comment: 
|         /*----- Subscribe Form -----*/
|     
|     Path: http://192.168.224.245:80/
|     Line number: 917
|     Comment: 
|         <!-- End Back To Top -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 459
|     Comment: 
|         /*----- Backgrounds ------*/
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 152
|     Comment: 
|         <!--[if "+(n||"")+" IE "+(t||"")+"]><a>&nbsp;</a><![endif]-->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 404
|     Comment: 
|         /*----- Typography -----*/
|     
|     Path: http://192.168.224.245:80/css/font-awesome/css/font-awesome.css
|     Line number: 23
|     Comment: 
|         /* makes the font 33% larger relative to the icon container */
|     
|     Path: http://192.168.224.245:80/
|     Line number: 369
|     Comment: 
|         <!-- Start About Section -->
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 951
|     Comment: 
|         /*Navbar Collapse Menu*/
|     
|     Path: http://192.168.224.245:80/js/plugins/revslider.min.js
|     Line number: 2
|     Comment: 
|         
|         
|         
|         *********************************************/
|     
|     Path: http://192.168.224.245:80/css/style.css
|     Line number: 3323
|     Comment: 
|_        /* fallback if grab cursor is unsupported */
| http-vhosts: 
| 90 names had status 200
|_38 names had status ERROR
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
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
|     MFC_Tear_Sample
|     PHPCrawl
|     URI::Fetch
|     Zend_Http_Client
|     http client
|     PECL::HTTP
|     Wget/1.13.4 (linux-gnu)
|_    WWW-Mechanize/1.34
| http-referer-checker: 
| Spidering limited to: maxpagecount=30
|_  http://maps.googleapis.com:80/maps/api/js
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-title: RELIA Corp.
|_http-chrono: Request times for /; avg: 1155.14ms; min: 664.76ms; max: 1645.09ms

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:01:25 2024 -- 1 IP address (1 host up) scanned in 150.39 seconds

```
