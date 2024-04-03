```bash
nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://192.168.224.245:8000 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nikto.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nikto.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nikto.txt):

```
- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          192.168.224.245
+ Target Hostname:    192.168.224.245
+ Target Port:        8000
+ Start Time:         2024-04-02 20:59:29 (GMT-7)
---------------------------------------------------------------------------
+ Server: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ Apache/2.4.49 appears to be outdated (current is at least Apache/2.4.54). Apache 2.2.34 is the EOL for the 2.x branch.
+ Python/3.8 appears to be outdated (current is at least 3.9.6).
+ OpenSSL/1.1.1f appears to be outdated (current is at least 3.0.7). OpenSSL 1.1.1s is current for the 1.x branch and will be supported until Nov 11 2023.
+ OPTIONS: Allowed HTTP Methods: GET, POST, OPTIONS, HEAD, TRACE .
+ /: HTTP TRACE method is active which suggests the host is vulnerable to XST. See: https://owasp.org/www-community/attacks/Cross_Site_Tracing
+ ERROR: Error limit (20) reached for host, giving up. Last error: 
+ Scan terminated: 0 error(s) and 7 item(s) reported on remote host
+ End Time:           2024-04-02 21:03:51 (GMT-7) (262 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested

```
