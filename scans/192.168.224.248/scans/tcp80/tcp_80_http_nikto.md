- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          192.168.224.248
+ Target Hostname:    192.168.224.248
+ Target Port:        80
+ Start Time:         2024-04-02 20:58:06 (GMT-7)
---------------------------------------------------------------------------
+ Server: No banner retrieved
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ /BbOd3iUr: Uncommon header 'x-result-reason' found, with contents: Not Redirected.
+ /BbOd3iUr: Uncommon header 'x-urlrewriter-404' found, with contents: 404 Rewritten to DNN Tab : 404 Error Page(Tabid:24) : Reason Requested_404.
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ /admin/: Uncommon header 'x-redirect-reason' found, with contents: Unfriendly Url 2 Requested.
+ /robots.txt: contains 16 entries which should be manually viewed. See: https://developer.mozilla.org/en-US/docs/Glossary/Robots.txt
+ OPTIONS: Allowed HTTP Methods: OPTIONS, TRACE, GET, HEAD, POST .
+ OPTIONS: Public HTTP Methods: OPTIONS, TRACE, GET, HEAD, POST .
+ /login/: This might be interesting.
+ /Portals/_default/Cache/ReadMe.txt: DotNetNuke default page found. Look for an admin interface on /tabid/19/, /tabid/36/ or enumerate numbers to identify logins/content.
+ 7748 requests: 0 error(s) and 9 item(s) reported on remote host
+ End Time:           2024-04-02 21:21:22 (GMT-7) (1396 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested
