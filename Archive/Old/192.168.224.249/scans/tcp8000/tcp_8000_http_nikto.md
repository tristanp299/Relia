- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          192.168.224.249
+ Target Hostname:    192.168.224.249
+ Target Port:        8000
+ Start Time:         2024-04-02 20:58:30 (GMT-7)
---------------------------------------------------------------------------
+ Server: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/7.4.30
+ /: Retrieved x-powered-by header: PHP/7.4.30.
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ Root page / redirects to: http://192.168.224.249/dashboard/
+ PHP/7.4.30 appears to be outdated (current is at least 8.1.5), PHP 7.4.28 for the 7.4 branch.
+ OpenSSL/1.1.1p appears to be outdated (current is at least 3.0.7). OpenSSL 1.1.1s is current for the 1.x branch and will be supported until Nov 11 2023.
+ /: HTTP TRACE method is active which suggests the host is vulnerable to XST. See: https://owasp.org/www-community/attacks/Cross_Site_Tracing
+ /img/: Directory indexing found.
+ /img/: This might be interesting.
+ /icons/: Directory indexing found.
+ /icons/README: Apache default file found. See: https://www.vntweb.co.uk/apache-restricting-access-to-iconsreadme/
+ /cms/: Cookie PHPSESSID created without the httponly flag. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies
+ /cms/: This might be interesting.
+ 8481 requests: 0 error(s) and 12 item(s) reported on remote host
+ End Time:           2024-04-02 21:20:06 (GMT-7) (1296 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested
