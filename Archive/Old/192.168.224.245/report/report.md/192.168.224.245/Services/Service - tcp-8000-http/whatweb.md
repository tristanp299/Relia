```bash
whatweb --color=never --no-errors -a 3 -v http://192.168.224.245:8000 2>&1
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_whatweb.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_whatweb.txt):

```
WhatWeb report for http://192.168.224.245:8000
Status    : 200 OK
Title     : <None>
IP        : 192.168.224.245
Country   : RESERVED, ZZ

Summary   : Apache[2.4.49][mod_wsgi/4.9.4], HTML5, HTTPServer[Unix][Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8], OpenSSL[1.1.1f], PasswordField[password], Python[3.8], Script

Detected Plugins:
[ Apache ]
	The Apache HTTP Server Project is an effort to develop and
	maintain an open-source HTTP server for modern operating
	systems including UNIX and Windows NT. The goal of this
	project is to provide a secure, efficient and extensible
	server that provides HTTP services in sync with the current
	HTTP standards.

	Version      : 2.4.49 (from HTTP Server Header)
	Module       : mod_wsgi/4.9.4
	Google Dorks: (3)
	Website     : http://httpd.apache.org/

[ HTML5 ]
	HTML version 5, detected by the doctype declaration


[ HTTPServer ]
	HTTP server header string. This plugin also attempts to
	identify the operating system from the server header.

	OS           : Unix
	String       : Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8 (from server string)

[ OpenSSL ]
	The OpenSSL Project is a collaborative effort to develop a
	robust, commercial-grade, full-featured, and Open Source
	toolkit implementing the Secure Sockets Layer (SSL v2/v3)
	and Transport Layer Security (TLS v1) protocols as well as
	a full-strength general purpose cryptography library.

	Version      : 1.1.1f
	Website     : http://www.openssl.org/

[ PasswordField ]
	find password fields

	String       : password (from field name)

[ Python ]
	Python is a programming language that lets you work more
	quickly and integrate your systems more effectively. You
	can learn to use Python and see almost immediate gains in
	productivity and lower maintenance costs.

	Version      : 3.8
	Website     : http://www.python.org/

[ Script ]
	This plugin detects instances of script HTML elements and
	returns the script language/type.


HTTP Headers:
	HTTP/1.1 200 OK
	Date: Wed, 03 Apr 2024 03:59:34 GMT
	Server: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
	Last-Modified: Wed, 12 Oct 2022 08:56:01 GMT
	ETag: "6ad-5ead28fdcdb81"
	Accept-Ranges: bytes
	Content-Length: 1709
	Connection: close
	Content-Type: text/html



```
