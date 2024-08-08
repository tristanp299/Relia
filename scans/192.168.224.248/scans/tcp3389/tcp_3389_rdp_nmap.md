# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:05 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 3389 "--script=banner,(rdp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp3389/tcp_3389_rdp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp3389/xml/tcp_3389_rdp_nmap.xml 192.168.224.248
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 20:58:06 PDT for 46s

PORT     STATE SERVICE       REASON          VERSION
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| rdp-enum-encryption: 
|   Security layer
|     CredSSP (NLA): SUCCESS
|     CredSSP with Early User Auth: SUCCESS
|     RDSTLS: SUCCESS
|     SSL: SUCCESS
|_  RDP Protocol Version: Unknown
|_ssl-date: 2024-04-03T03:58:34+00:00; 0s from scanner time.
| rdp-ntlm-info: 
|   Target_Name: EXTERNAL
|   NetBIOS_Domain_Name: EXTERNAL
|   NetBIOS_Computer_Name: EXTERNAL
|   DNS_Domain_Name: EXTERNAL
|   DNS_Computer_Name: EXTERNAL
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T03:58:13+00:00
| ssl-enum-ciphers: 
|   TLSv1.0: 
|     ciphers: 
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|     compressors: 
|       NULL
|     cipher preference: server
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
|       TLS_RSA_WITH_AES_256_GCM_SHA384 (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_GCM_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|       TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 (ecdh_x25519) - A
|       TLS_DHE_RSA_WITH_AES_256_GCM_SHA384 (dh 2048) - A
|       TLS_DHE_RSA_WITH_AES_128_GCM_SHA256 (dh 2048) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384 (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256 (ecdh_x25519) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|     compressors: 
|       NULL
|     cipher preference: server
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|_  least strength: C
| ssl-cert: Subject: commonName=EXTERNAL
| Issuer: commonName=EXTERNAL
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-04-02T03:51:10
| Not valid after:  2024-10-02T03:51:10
| MD5:   a584:bf4a:b48c:d730:436b:18f8:820a:32ee
| SHA-1: 5c85:e2ad:976d:8022:e913:8ab9:d6c4:333e:c6b8:5311
| -----BEGIN CERTIFICATE-----
| MIIC1DCCAbygAwIBAgIQFve+lwKgxrBIfE+bDvTHbDANBgkqhkiG9w0BAQsFADAT
| MREwDwYDVQQDEwhFWFRFUk5BTDAeFw0yNDA0MDIwMzUxMTBaFw0yNDEwMDIwMzUx
| MTBaMBMxETAPBgNVBAMTCEVYVEVSTkFMMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8A
| MIIBCgKCAQEA56oZDQTDXOkiRVHOam3X3cCkYXmnyUzkGgfj3d/ivGFrGXSwqF8R
| Yo6R0GtTDAnA/mDXxPMVIZn6X4R8e+OBjI3l33auLZlulnbVcVV14U7wD7MDdmxi
| vUO/rGLgQiM4S2kqRbV/TFIY8lLkeQm8pyusEK2SR/d6ePd/w5SgHQayqmbtTvB9
| VtdMJyqf47A2WkGfp0DbvfUVvXQokekP6wc9uEjRwvJXYf6qRN1MyrcbZwkROQ+d
| 7YIkIlyDqPF0zlCmlrDtfAxaqJYzQxRAJ1N1SPXwGSd2vFg21kKEhtAdGJnA7B2I
| p2hBv0tM32KGjOCm6lLNgdMQt7VHFu/8ZQIDAQABoyQwIjATBgNVHSUEDDAKBggr
| BgEFBQcDATALBgNVHQ8EBAMCBDAwDQYJKoZIhvcNAQELBQADggEBAFislqelLcB7
| VzIbb+Ch9dEEJIz99tcgpZLw3jT8aEHvLtrH6XAZ1bj3UjWS+RnoXfBOpB7PAYw4
| SQIyeJb0chLBEdS/OsATF7wEMS/oaHM2fCHYcVBH6+ZR+bmeswJMNFBeSPA1TzB4
| xPMZUc7Jq3rLepXmoZRoIzIKAoYZRr7eXpJtpO3U4P6seM3abdRbjdzduE5GjARt
| nqb+qFhLRu9nkxV9EIWTj0qlfNPzTB4Gg9+El/DMcMaEXTJU/gxQ2XKHut6yWSdk
| H4MtV5ENWDn4hGip+g5AoXgy6KF6s10FBkNZPpEdM14c8wjQwJeMMQINxryw6p/r
| Y6br6Wk8ydg=
|_-----END CERTIFICATE-----
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:52 2024 -- 1 IP address (1 host up) scanned in 46.66 seconds
