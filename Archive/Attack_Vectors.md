#### Potential
192.168.224.249

80/tcp   open  http          syn-ack Microsoft IIS httpd 10.0
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
|_http-title: IIS Windows Server
|_http-server-header: Microsoft-IIS/10.0
135/tcp  open  msrpc         syn-ack Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? syn-ack
3389/tcp open  ms-wbt-server syn-ack Microsoft Terminal Services
| ssl-cert: Subject: commonName=LEGACY
| rdp-ntlm-info: 
|   Target_Name: LEGACY
|   NetBIOS_Domain_Name: LEGACY
|   NetBIOS_Computer_Name: LEGACY
|   DNS_Domain_Name: LEGACY
|   DNS_Computer_Name: LEGACY
|   Product_Version: 10.0.20348
8000/tcp open  http          syn-ack Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/7.4.30)
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/7.4.30
|_Requested resource was http://192.168.224.249:8000/dashboard/
|_http-open-proxy: Proxy might be redirecting requests
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

192.168.224.248
80/tcp   open  http          syn-ack Microsoft IIS httpd 10.0
| http-robots.txt: 16 disallowed entries 
| /*/ctl/ /admin/ /App_Browsers/ /App_Code/ /App_Data/ 
| /App_GlobalResources/ /bin/ /Components/ /Config/ /contest/ /controls/ 
| /Documentation/ /HttpModules/ /Install/ /Providers/ 
|_/Activity-Feed/userId/
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
135/tcp  open  msrpc         syn-ack Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? syn-ack
3389/tcp open  ms-wbt-server syn-ack Microsoft Terminal Services
| ssl-cert: Subject: commonName=EXTERNAL
| rdp-ntlm-info: 
|   Target_Name: EXTERNAL
|   NetBIOS_Domain_Name: EXTERNAL
|   NetBIOS_Computer_Name: EXTERNAL
|   DNS_Domain_Name: EXTERNAL
|   DNS_Computer_Name: EXTERNAL
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T03:55:32+00:00
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

192.168.224.247
80/tcp   open  http          syn-ack Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-title: RELIA - New Hire Information
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
135/tcp  open  msrpc         syn-ack Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
443/tcp  open  ssl/http      syn-ack Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
| ssl-cert: Subject: commonName=localhost
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
| tls-alpn: 
|_  http/1.1
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
445/tcp  open  microsoft-ds? syn-ack
3389/tcp open  ms-wbt-server syn-ack Microsoft Terminal Services

192.168.224.247
80/tcp   open  http          syn-ack Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-title: RELIA - New Hire Information
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
135/tcp  open  msrpc         syn-ack Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
443/tcp  open  ssl/http      syn-ack Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/8.1.10)
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
|_http-title: RELIA - New Hire Information
| ssl-cert: Subject: commonName=localhost
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/8.1.10
| tls-alpn: 
|_  http/1.1
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
445/tcp  open  microsoft-ds? syn-ack
3389/tcp open  ms-wbt-server syn-ack Microsoft Terminal Services
|_ssl-date: 2024-04-03T03:56:21+00:00; 0s from scanner time.
| ssl-cert: Subject: commonName=WEB02
| Issuer: commonName=WEB02
| rdp-ntlm-info: 
|   Target_Name: WEB02
|   NetBIOS_Domain_Name: WEB02
|   NetBIOS_Computer_Name: WEB02
|   DNS_Domain_Name: WEB02
|   DNS_Computer_Name: WEB02
|   Product_Version: 10.0.20348

192.168.224.246
80/tcp   open  http     syn-ack Apache httpd 2.4.52 ((Ubuntu))
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-server-header: Apache/2.4.52 (Ubuntu)
|_http-title: Code Validation
443/tcp  open  ssl/http syn-ack Apache httpd 2.4.52 ((Ubuntu))
|_http-title: Code Validation
|_http-server-header: Apache/2.4.52 (Ubuntu)
| ssl-cert: Subject: commonName=demo
| tls-alpn: 
|_  http/1.1
|_ssl-date: TLS randomness does not represent time
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
2222/tcp open  ssh      syn-ack OpenSSH 8.9p1 UbuntuService Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel 3 (Ubuntu Linux; protocol 2.0)
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

192.168.224.245
21/tcp   open  ftp      syn-ack vsftpd 2.0.8 or later
|_ftp-anon: Anonymous FTP login allowed (FTP code 230)
|      vsFTPd 3.0.3 - secure, fast, stable
80/tcp   open  http     syn-ack Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
|_http-title: RELIA Corp.
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
443/tcp  open  ssl/http syn-ack Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
| ssl-cert: Subject: commonName=web01.relia.com/organizationName=RELIA/stateOrProvinceName=Berlin/countryName=DE/localityName=Munich/organizationalUnitName=IT Department
localityName=Munich/organizationalUnitName=IT Department
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
|_http-title: RELIA Corp.
2222/tcp open  ssh      syn-ack OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
8000/tcp open  http     syn-ack Apache httpd 2.4.49 ((Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8)
|_http-title: Site doesn't have a title (text/html).
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
Service Info: Host: RELIA; OS: Linux; CPE: cpe:/o:linux:linux_kernel

192.168.224.191
80/tcp   open  http          syn-ack Microsoft IIS httpd 10.0
| http-auth: 
| HTTP/1.1 401 Unauthorized\x0D
|_  Basic realm=192.168.224.191
|_http-server-header: Microsoft-IIS/10.0
|_http-title: 401 - Unauthorized: Access is denied due to invalid credentials.
135/tcp  open  msrpc         syn-ack Microsoft Windows RPC
139/tcp  open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? syn-ack
3389/tcp open  ms-wbt-server syn-ack Microsoft Terminal Services
| rdp-ntlm-info: 
|   Target_Name: RELIA
|   NetBIOS_Domain_Name: RELIA
|   NetBIOS_Computer_Name: LOGIN
|   DNS_Domain_Name: relia.com
|   DNS_Computer_Name: login.relia.com
|   DNS_Tree_Name: relia.com
|   Product_Version: 10.0.20348
| ssl-cert: Subject: commonName=login.relia.com
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

192.168.224.189
25/tcp  open  smtp          syn-ack hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
110/tcp open  pop3          syn-ack hMailServer pop3d
|_pop3-capabilities: USER TOP UIDL
135/tcp open  msrpc         syn-ack Microsoft Windows RPC
139/tcp open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
143/tcp open  imap          syn-ack hMailServer imapd
|_imap-capabilities: completed IDLE NAMESPACE CHILDREN QUOTA RIGHTS=texkA0001 ACL SORT CAPABILITY OK IMAP4 IMAP4rev1
445/tcp open  microsoft-ds? syn-ack
587/tcp open  smtp          syn-ack hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
Service Info: Host: MAIL; OS: Windows; CPE: cpe:/o:microsoft:windows

192.168.224.250
135/tcp  open  msrpc              syn-ack Microsoft Windows RPC
139/tcp  open  netbios-ssn        syn-ack Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?      syn-ack
3389/tcp open  ssl/ms-wbt-server? syn-ack
|_ssl-date: 2024-04-03T03:56:21+00:00; 0s from scanner time.
| rdp-ntlm-info: 
|   Target_Name: WINPREP
|   NetBIOS_Domain_Name: WINPREP
|   NetBIOS_Computer_Name: WINPREP
|   DNS_Domain_Name: WINPREP
|   DNS_Computer_Name: WINPREP
| ssl-cert: Subject: commonName=WINPREP
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows




#### High Potential
- 192.168.224.249
8000/tcp open  http          syn-ack Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/7.4.30)
- 192.168.224.245
21/tcp   open  ftp      syn-ack vsftpd 2.0.8 or later
|_ftp-anon: Anonymous FTP login allowed (FTP code 230)
|      vsFTPd 3.0.3 - secure, fast, stable
|_http-server-header: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
2222/tcp open  ssh      syn-ack OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
- 192.168.224.189
25/tcp  open  smtp          syn-ack hMailServer smtpd
| smtp-commands: MAIL, SIZE 20480000, AUTH LOGIN, HELP
|_ 211 DATA HELO EHLO MAIL NOOP QUIT RCPT RSET SAML TURN VRFY
- 192.168.224.189
SMTP / IMAP
- 192.168.224.250
RDP -> offsec:labs
#### Failed

#### Successful

#### Target Information




