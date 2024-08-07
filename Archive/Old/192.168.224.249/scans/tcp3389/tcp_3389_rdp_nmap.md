# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:08 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 3389 "--script=banner,(rdp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.249/scans/tcp3389/tcp_3389_rdp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.249/scans/tcp3389/xml/tcp_3389_rdp_nmap.xml 192.168.224.249
Nmap scan report for 192.168.224.249
Host is up, received user-set (0.079s latency).
Scanned at 2024-04-02 20:58:08 PDT for 50s

PORT     STATE SERVICE       REASON          VERSION
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| ssl-cert: Subject: commonName=LEGACY
| Issuer: commonName=LEGACY
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-01-13T23:01:30
| Not valid after:  2024-07-14T23:01:30
| MD5:   ced0:46fb:0382:2c78:4f8e:6e99:7ce2:feaa
| SHA-1: 5931:bfe6:185b:7084:5964:45fb:b55a:3383:85b3:9f7f
| -----BEGIN CERTIFICATE-----
| MIIC0DCCAbigAwIBAgIQYUbza/e+y6VDeQQningixDANBgkqhkiG9w0BAQsFADAR
| MQ8wDQYDVQQDEwZMRUdBQ1kwHhcNMjQwMTEzMjMwMTMwWhcNMjQwNzE0MjMwMTMw
| WjARMQ8wDQYDVQQDEwZMRUdBQ1kwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEK
| AoIBAQCqwka8tAMwtxNQW84u3c2UTguRuAqMNN/4StHyBwGRYKaMS+TfJC/HaWqN
| F0szmrm0L2wTibd/Ndj29TZV0jVOfkTroDoriaHlpjo+cFA6t46e6p0gzuW0K0NK
| 8Npn7FgtlVNgtV8NUvqYq0Juu+z0EhscYh7GhuCdcDLZ1tK6/ehBQkFW96JWpaWo
| Hwus91+dtveOUGxU5+V1UpvW3OkboxoK6Z3bKiqdnevSi5O79BFl9KOQsPJlgwNW
| k8tkWrpAWiSldsNgQ1ZHbKETPdQLFKLPmD0mb8ycw5OIxsaKTwdVbFu/g70UlN5W
| CsMuUJnTiFGpOSHljGDAa7PhN6NVAgMBAAGjJDAiMBMGA1UdJQQMMAoGCCsGAQUF
| BwMBMAsGA1UdDwQEAwIEMDANBgkqhkiG9w0BAQsFAAOCAQEAaUqBAi7tO/D2ZVTy
| N9zEVSnrKvZQ3mJSQNd7Tykw9q4vuMYqmziwd1zrkALTxmWOJ70YTaR14DxQFZ/0
| 9+9TY8d3aeAcA+JxMeSDbXcE2FNCKV8CBc/iD5dUIr+wF3Psb6Va1l3636Al1g9x
| NUMtGoJhfnuxERQOyR+HioGz8dtnK+GSaSfa+4r7jYUySuIL405Cgk0PDPs29D3F
| BrTvzgZsYu8L4tZMOhD8LMMEFQ7axISAUNBRXnAI5/kOkdoCe5m/KMpzIsFi5Pyj
| MPNRNYsGnI+RGBgUpPgtVDGWIvRRkzZ+Ogqw3CUaR9NaxrOLtPMvNjrgUGpd9RR5
| VvEnKg==
|_-----END CERTIFICATE-----
| rdp-enum-encryption: 
|   Security layer
|     CredSSP (NLA): SUCCESS
|     CredSSP with Early User Auth: SUCCESS
|_    RDSTLS: SUCCESS
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
| rdp-ntlm-info: 
|   Target_Name: LEGACY
|   NetBIOS_Domain_Name: LEGACY
|   NetBIOS_Computer_Name: LEGACY
|   DNS_Domain_Name: LEGACY
|   DNS_Computer_Name: LEGACY
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T03:58:17+00:00
|_ssl-date: 2024-04-03T03:58:38+00:00; 0s from scanner time.
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:58:58 2024 -- 1 IP address (1 host up) scanned in 50.44 seconds
