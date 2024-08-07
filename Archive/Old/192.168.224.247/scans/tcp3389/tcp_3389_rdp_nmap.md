# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:32 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 3389 "--script=banner,(rdp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp3389/tcp_3389_rdp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp3389/xml/tcp_3389_rdp_nmap.xml 192.168.224.247
Nmap scan report for 192.168.224.247
Host is up, received user-set (0.093s latency).
Scanned at 2024-04-02 20:58:32 PDT for 61s

PORT     STATE SERVICE       REASON          VERSION
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| ssl-cert: Subject: commonName=WEB02
| Issuer: commonName=WEB02
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-04-02T03:51:09
| Not valid after:  2024-10-02T03:51:09
| MD5:   f22b:9bf1:9594:98da:b395:098d:f202:d2cf
| SHA-1: 832f:3545:10e1:9ae2:9511:7e8c:70ba:bf11:931e:0440
| -----BEGIN CERTIFICATE-----
| MIICzjCCAbagAwIBAgIQMBzqK4I/dYZGHyAZ1HsbEDANBgkqhkiG9w0BAQsFADAQ
| MQ4wDAYDVQQDEwVXRUIwMjAeFw0yNDA0MDIwMzUxMDlaFw0yNDEwMDIwMzUxMDla
| MBAxDjAMBgNVBAMTBVdFQjAyMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKC
| AQEAp01R4pjmdmISv24hs9qEOM2/O3Sz6H7b2xSU7CiCOVnzwc7hJaP5raJFd0am
| 18xDRiOlB4Qks6+snvVeDj/j/gLZh4G4bwfD2G8Wp5lEkwkCQ0qQeMnPaVZxcKM6
| 8BUrYYPwyjFTczXWE2d/7Prinx7xUsjbZrPy7SqqSxXtIeWoUxAuW+vw6dF/TEPZ
| ZM4sOD170dolr5bOcRCEtRDMYUeZSVAHZBTwL5RBuh6qPyEdLhRWS5tLTn374KUS
| Ydse3J7+OrItNpwbBj44ziYmSbPwahfZbhwxWvGGIKbb3KOsrFyvPjT11bk6klz8
| KlT+5ab1Sloc0xCiDiHiMCT8zQIDAQABoyQwIjATBgNVHSUEDDAKBggrBgEFBQcD
| ATALBgNVHQ8EBAMCBDAwDQYJKoZIhvcNAQELBQADggEBAGm9FpqKXZDsW5m2iG5w
| 6sgDJhlv6GSuke7Y6QkiOWajoYxkXUNeCW2l/mzeLE8r5ZIiyKRAD/fWKVWT0dE8
| xd26juMctbXQNhQZ3rTan/p9JylF0crpij70NsapWS8EKUwiYShT0MWXP49ghOPz
| hHvzLCCgHkpLCAgH/AfWe7U8hbscivpgoPT8czyz6LpuB+jXxezvMa+/qEiUs7od
| 5rDivHnA2uNvflShfardw92SIFi+/0Cd8D9wPunM2AvhDuM8H0XrwKcXBjGtCJdg
| rGwHwexpRgwr4y5mzujqI/OupEiU8wMMYxxMS7IFPz+C5XNWWjhyvN+LRtmM2Jvh
| BOQ=
|_-----END CERTIFICATE-----
| rdp-enum-encryption: 
|   Security layer
|     CredSSP (NLA): SUCCESS
|     CredSSP with Early User Auth: SUCCESS
|     RDSTLS: SUCCESS
|     SSL: SUCCESS
|_  RDP Protocol Version: Unknown
| ssl-enum-ciphers: 
|   TLSv1.0: 
|     ciphers: 
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|     compressors: 
|       NULL
|     cipher preference: server
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|   TLSv1.1: 
|     ciphers: 
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|     compressors: 
|       NULL
|     cipher preference: server
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|   TLSv1.2: 
|     ciphers: 
|       TLS_DHE_RSA_WITH_AES_128_GCM_SHA256 (dh 2048) - A
|       TLS_DHE_RSA_WITH_AES_256_GCM_SHA384 (dh 2048) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256 (ecdh_x25519) - A
|       TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 (ecdh_x25519) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384 (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 (secp384r1) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_GCM_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_GCM_SHA384 (rsa 2048) - A
|     compressors: 
|       NULL
|     cipher preference: server
|     cipher preference error: Network error
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|_  least strength: C
| rdp-ntlm-info: 
|   Target_Name: WEB02
|   NetBIOS_Domain_Name: WEB02
|   NetBIOS_Computer_Name: WEB02
|   DNS_Domain_Name: WEB02
|   DNS_Computer_Name: WEB02
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T03:58:39+00:00
|_ssl-date: 2024-04-03T03:58:59+00:00; 0s from scanner time.
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:59:33 2024 -- 1 IP address (1 host up) scanned in 60.77 seconds
