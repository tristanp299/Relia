```bash
nikto -ask=no -Tuning=x4567890ac -nointeractive -host https://192.168.224.246:443 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nikto.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nikto.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_nikto.txt):

```
- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          192.168.224.246
+ Target Hostname:    192.168.224.246
+ Target Port:        443
---------------------------------------------------------------------------
+ SSL Info:        Subject:  /CN=demo
                   Ciphers:  TLS_AES_256_GCM_SHA384
                   Issuer:   /CN=demo
+ Start Time:         2024-04-02 21:01:04 (GMT-7)
---------------------------------------------------------------------------
+ Server: Apache/2.4.52 (Ubuntu)
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The site uses TLS and the Strict-Transport-Security HTTP header is not defined. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ ERROR: Error limit (20) reached for host, giving up. Last error: 
+ Scan terminated: 7 error(s) and 3 item(s) reported on remote host
+ End Time:           2024-04-02 21:14:17 (GMT-7) (793 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested

```
