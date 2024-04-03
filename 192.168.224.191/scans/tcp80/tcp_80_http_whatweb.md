WhatWeb report for http://192.168.224.191:80
Status    : 401 Unauthorized
Title     : 401 - Unauthorized: Access is denied due to invalid credentials.
IP        : 192.168.224.191
Country   : RESERVED, ZZ

Summary   : HTTPServer[Microsoft-IIS/10.0], Microsoft-IIS[10.0], WWW-Authenticate[192.168.224.191][Basic]

Detected Plugins:
[ HTTPServer ]
	HTTP server header string. This plugin also attempts to
	identify the operating system from the server header.

	String       : Microsoft-IIS/10.0 (from server string)

[ Microsoft-IIS ]
	Microsoft Internet Information Services (IIS) for Windows
	Server is a flexible, secure and easy-to-manage Web server
	for hosting anything on the Web. From media streaming to
	web application hosting, IIS's scalable and open
	architecture is ready to handle the most demanding tasks.

	Version      : 10.0
	Website     : http://www.iis.net/

[ WWW-Authenticate ]
	This plugin identifies the WWW-Authenticate HTTP header and
	extracts the authentication method and realm.

	Module       : Basic
	String       : 192.168.224.191

HTTP Headers:
	HTTP/1.1 401 Unauthorized
	Content-Type: text/html
	Server: Microsoft-IIS/10.0
	WWW-Authenticate: Basic realm="192.168.224.191"
	Date: Wed, 03 Apr 2024 04:09:07 GMT
	Connection: close
	Content-Length: 1293


