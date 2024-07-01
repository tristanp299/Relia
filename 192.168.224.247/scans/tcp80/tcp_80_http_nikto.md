- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          192.168.224.247
+ Target Hostname:    192.168.224.247
+ Target Port:        80
+ Start Time:         2024-04-02 20:58:10 (GMT-7)
---------------------------------------------------------------------------
+ Server: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
+ /: Retrieved x-powered-by header: PHP/8.1.10.
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ OpenSSL/1.1.1p appears to be outdated (current is at least 3.0.7). OpenSSL 1.1.1s is current for the 1.x branch and will be supported until Nov 11 2023.
+ /: Web Server returns a valid response with junk HTTP methods which may cause false positives.
+ /: HTTP TRACE method is active which suggests the host is vulnerable to XST. See: https://owasp.org/www-community/attacks/Cross_Site_Tracing
+ ERROR: Error limit (20) reached for host, giving up. Last error: opening stream: can't connect (timeout): Transport endpoint is not connected
+ Scan terminated: 11 error(s) and 6 item(s) reported on remote host
+ End Time:           2024-04-02 21:09:40 (GMT-7) (690 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested
