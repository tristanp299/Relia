- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          192.168.224.246
+ Target Hostname:    192.168.224.246
+ Target Port:        80
+ Start Time:         2024-04-02 20:57:14 (GMT-7)
---------------------------------------------------------------------------
+ Server: Apache/2.4.52 (Ubuntu)
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ Apache/2.4.52 appears to be outdated (current is at least Apache/2.4.54). Apache 2.2.34 is the EOL for the 2.x branch.
+ /: Web Server returns a valid response with junk HTTP methods which may cause false positives.
+ /: DEBUG HTTP verb may show server debugging information. See: https://docs.microsoft.com/en-us/visualstudio/debugger/how-to-enable-debugging-for-aspnet-applications?view=vs-2017
+ /submit?setoption=q&option=allowed_ips&value=255.255.255.255: IP address found in the 'location' header. The IP is "255.255.255.255". See: https://portswigger.net/kb/issues/00600300_private-ip-addresses-disclosed
+ /css/: Directory indexing found.
+ /css/: This might be interesting.
+ 7742 requests: 10 error(s) and 8 item(s) reported on remote host
+ End Time:           2024-04-02 21:19:51 (GMT-7) (1357 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested
