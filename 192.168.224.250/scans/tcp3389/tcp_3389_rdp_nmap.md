# Nmap 7.94SVN scan initiated Tue Apr  2 21:11:59 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 3389 "--script=banner,(rdp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.250/scans/tcp3389/tcp_3389_rdp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.250/scans/tcp3389/xml/tcp_3389_rdp_nmap.xml 192.168.224.250
Nmap scan report for 192.168.224.250
Host is up, received user-set (0.098s latency).
Scanned at 2024-04-02 21:11:59 PDT for 89s

PORT     STATE SERVICE            REASON          VERSION
3389/tcp open  ssl/ms-wbt-server? syn-ack ttl 125
| ssl-cert: Subject: commonName=WINPREP
| Issuer: commonName=WINPREP
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-03-07T05:25:18
| Not valid after:  2024-09-06T05:25:18
| MD5:   51fe:9a6b:977e:78b5:d2d2:35a0:4b19:cb0a
| SHA-1: 9ec8:635a:9ebb:0933:560e:50e5:16ed:948c:4b98:430d
| -----BEGIN CERTIFICATE-----
| MIIC0jCCAbqgAwIBAgIQVyQ8hwp5ja5On/WxoMbIQzANBgkqhkiG9w0BAQsFADAS
| MRAwDgYDVQQDEwdXSU5QUkVQMB4XDTI0MDMwNzA1MjUxOFoXDTI0MDkwNjA1MjUx
| OFowEjEQMA4GA1UEAxMHV0lOUFJFUDCCASIwDQYJKoZIhvcNAQEBBQADggEPADCC
| AQoCggEBALgBTSknRu2n0JD9KIyDYjk/bFfD5N7iY4IQ6/+tgkzTO7N3LfpMn0iB
| y4El/3mwFEZk58RSrbxfbuBmKTN7U3k1skhoOt7tK557/Nbl81M/YM2QqzmT8Kho
| WHXLo5bI1ePY+VZHkgLBvWuNohutkcLnnADFO/9YvaWorPBcB43T6630cfPCLYJC
| xTSXOYKMmVG/mu79fbwZDng44QmAKGJjIpmU9a+OJCZEsHE5DwMav+V2HWjiUrU4
| 47JdUqOMpetrPp/BsE4ztCBlD5qXVQAycNYzjyXCtu//DwpZfNhS+RExkxjX34X9
| syVhpIJnvsfOdKFwH5lBIzf1YrT2dd0CAwEAAaMkMCIwEwYDVR0lBAwwCgYIKwYB
| BQUHAwEwCwYDVR0PBAQDAgQwMA0GCSqGSIb3DQEBCwUAA4IBAQB2BaKxWEpYJ+Lb
| slcgSZcKq+NHYZMYexA8Ip+1j44zsAKdfH3cfTEh3gMGNxjWRuW7K0Zr2/enIcKW
| LmyH7M2Nqz3c9+g7jR7Rt8uhniHVrF59A0fMw+HTEs9ofDIFU92ap1Yn/bx51cC3
| ITCXykxjDvnb4oiqkIMolps3fC71Y4+f9TXeHoOMSoJ0PQqS9eqC/bnWanpWhTVQ
| LGGGTk071eHTvP5jxUOe/nqDs5HYzqktcp3DAf7QtcL38a0csZmMFg6MWrMTcdWB
| jsx1a0FUIf9Qk+00n7dlipCnT7MwGqMwH6n1njs/Zsvkh90oRgE5Ett95gX3L5B9
| KiBcAO4P
|_-----END CERTIFICATE-----
| rdp-enum-encryption: 
|   Security layer
|     CredSSP (NLA): SUCCESS
|     CredSSP with Early User Auth: SUCCESS
|_    RDSTLS: SUCCESS
| rdp-ntlm-info: 
|   Target_Name: WINPREP
|   NetBIOS_Domain_Name: WINPREP
|   NetBIOS_Computer_Name: WINPREP
|   DNS_Domain_Name: WINPREP
|   DNS_Computer_Name: WINPREP
|   Product_Version: 10.0.22000
|_  System_Time: 2024-04-03T04:12:49+00:00
|_ssl-date: 2024-04-03T04:13:10+00:00; 0s from scanner time.
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

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:13:28 2024 -- 1 IP address (1 host up) scanned in 89.40 seconds
