```bash
whatweb --color=never --no-errors -a 3 -v https://192.168.224.246:443 2>&1
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_whatweb.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_whatweb.txt):

```
WhatWeb report for https://192.168.224.246:443
Status    : 200 OK
Title     : Code Validation
IP        : 192.168.224.246
Country   : RESERVED, ZZ

Summary   : Apache[2.4.52], HTML5, HTTPServer[Ubuntu Linux][Apache/2.4.52 (Ubuntu)], JQuery[1.12.4], Script

Detected Plugins:
[ Apache ]
	The Apache HTTP Server Project is an effort to develop and
	maintain an open-source HTTP server for modern operating
	systems including UNIX and Windows NT. The goal of this
	project is to provide a secure, efficient and extensible
	server that provides HTTP services in sync with the current
	HTTP standards.

	Version      : 2.4.52 (from HTTP Server Header)
	Google Dorks: (3)
	Website     : http://httpd.apache.org/

[ HTML5 ]
	HTML version 5, detected by the doctype declaration


[ HTTPServer ]
	HTTP server header string. This plugin also attempts to
	identify the operating system from the server header.

	OS           : Ubuntu Linux
	String       : Apache/2.4.52 (Ubuntu) (from server string)

[ JQuery ]
	A fast, concise, JavaScript that simplifies how to traverse
	HTML documents, handle events, perform animations, and add
	AJAX.

	Version      : 1.12.4
	Website     : http://jquery.com/

[ Script ]
	This plugin detects instances of script HTML elements and
	returns the script language/type.


HTTP Headers:
	HTTP/1.1 200 OK
	Date: Wed, 03 Apr 2024 04:01:04 GMT
	Server: Apache/2.4.52 (Ubuntu)
	Vary: Accept-Encoding
	Content-Encoding: gzip
	Content-Length: 659
	Connection: close
	Content-Type: text/html; charset=UTF-8



```
