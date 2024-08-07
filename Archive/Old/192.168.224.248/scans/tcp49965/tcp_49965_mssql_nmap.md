# Nmap 7.94SVN scan initiated Tue Apr  2 21:05:09 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 49965 "--script=banner,(ms-sql* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" --script-args=mssql.instance-port=49965,mssql.username=sa,mssql.password=sa -oN /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp49965/tcp_49965_mssql_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.248/scans/tcp49965/xml/tcp_49965_mssql_nmap.xml 192.168.224.248
Nmap scan report for 192.168.224.248
Host is up, received user-set (0.11s latency).
Scanned at 2024-04-02 21:05:09 PDT for 85s

Bug in ms-sql-dac: no string output.
Bug in ms-sql-hasdbaccess: no string output.
PORT      STATE SERVICE  REASON          VERSION
49965/tcp open  ms-sql-s syn-ack ttl 125 Microsoft SQL Server 2019 15.00.2000.00; RTM
| ssl-enum-ciphers: 
|   TLSv1.0: 
|     ciphers: 
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|     compressors: 
|       NULL
|     cipher preference: server
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|   TLSv1.1: 
|     ciphers: 
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|     compressors: 
|       NULL
|     cipher preference: server
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|   TLSv1.2: 
|     ciphers: 
|       TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 (ecdh_x25519) - A
|       TLS_DHE_RSA_WITH_AES_256_GCM_SHA384 (dh 2048) - A
|       TLS_DHE_RSA_WITH_AES_128_GCM_SHA256 (dh 2048) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384 (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256 (ecdh_x25519) - A
|       TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (secp384r1) - A
|       TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (ecdh_x25519) - A
|       TLS_RSA_WITH_AES_256_GCM_SHA384 (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_GCM_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA256 (rsa 2048) - A
|       TLS_RSA_WITH_AES_256_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_AES_128_CBC_SHA (rsa 2048) - A
|       TLS_RSA_WITH_3DES_EDE_CBC_SHA (rsa 2048) - C
|     compressors: 
|       NULL
|     cipher preference: server
|     warnings: 
|       64-bit block cipher 3DES vulnerable to SWEET32 attack
|_  least strength: C
| ms-sql-tables: 
|   192.168.224.248:49965: 
|_[192.168.224.248:49965]
| ms-sql-empty-password: 
|   192.168.224.248:49965: 
|_    'sa' account password is not blank.
| ms-sql-dump-hashes: 
|_  192.168.224.248:49965: ERROR: Bad username or password
| ms-sql-query: 
|_  (Use --script-args=ms-sql-query.query='<QUERY>' to change query.)
| ssl-cert: Subject: commonName=SSL_Self_Signed_Fallback
| Issuer: commonName=SSL_Self_Signed_Fallback
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2023-03-01T06:42:58
| Not valid after:  2053-03-01T06:42:58
| MD5:   022f:e745:145a:cada:c06e:cb13:239b:465d
| SHA-1: a905:ee65:7daa:11d2:a294:82d2:b3c9:3b94:6d72:9373
| -----BEGIN CERTIFICATE-----
| MIIDADCCAeigAwIBAgIQOtQrLNfn+IhF0ZXlptCaojANBgkqhkiG9w0BAQsFADA7
| MTkwNwYDVQQDHjAAUwBTAEwAXwBTAGUAbABmAF8AUwBpAGcAbgBlAGQAXwBGAGEA
| bABsAGIAYQBjAGswIBcNMjMwMzAxMDY0MjU4WhgPMjA1MzAzMDEwNjQyNThaMDsx
| OTA3BgNVBAMeMABTAFMATABfAFMAZQBsAGYAXwBTAGkAZwBuAGUAZABfAEYAYQBs
| AGwAYgBhAGMAazCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEBAOGZFIF+
| tnPKxnC2Ac0Gtn/pM812NYNpaqxNImrILilpHDIVxklXE7EiO3PLfsB9mtAKeXKh
| 2NpPN0CN4p8Oe1LyozKJuHKpf9B4xgHHrU7WM2h8XU4zGmPvQ4j3ULfh+3jkr1Xm
| hboAUze5IMrUomdtU2224c+aI2vSVJOLKZ2n6iaBbpFVx26wcJp/D5ATKwoHu+fq
| g0UScRl8ElU0qx17zs2HtmQIXSV83wg7IatAturL4cmULjKrtPTzIsImOjtXzKdP
| +Mj7uYP8Akfr9xNazgcBYvivLEn1v60k80vOL49gWa/gmk0/P8A2tHvkWsGRbq0R
| 3+GNAjhdlLUBHt0CAwEAATANBgkqhkiG9w0BAQsFAAOCAQEAVu1e7C+HcvZiN1OV
| eNKcgwU0VLEh4nkKwLHJ8HfdCEZ79YscSVuk042QN0FFVUuNZR9SwiYb9wY+pjvj
| 2NpDrK7UcgYTXZY4nXZLC+pTurcBC24nD3ZE38RGJnXkt9lW1WSbCBX2/QaQHeCT
| dEUoWGy5DAo0f0AwUHK2Q+5diuqjwD1gAgJEy3GsjQOUym99Qc+iP7a4c8qbvLdS
| SY+zgQFfrqmKsZ/LKI7ypPa1uorDneCSH7uhr67mqWgGMfDOn4D9g/U9q3TM7lLN
| tb/yIgCrlIaoAmFep+qbMquxa7kh4M6NnkINsuD/QESDEb0z1lqhB6ZOhDWCq/to
| dtwIrQ==
|_-----END CERTIFICATE-----
| ms-sql-ntlm-info: 
|   192.168.224.248:49965: 
|     Target_Name: EXTERNAL
|     NetBIOS_Domain_Name: EXTERNAL
|     NetBIOS_Computer_Name: EXTERNAL
|     DNS_Domain_Name: EXTERNAL
|     DNS_Computer_Name: EXTERNAL
|_    Product_Version: 10.0.20348
| ms-sql-info: 
|   192.168.224.248:49965: 
|     Version: 
|       name: Microsoft SQL Server 2019 RTM
|       number: 15.00.2000.00
|       Product: Microsoft SQL Server 2019
|       Service pack level: RTM
|       Post-SP patches applied: false
|_    TCP port: 49965
| ms-sql-xp-cmdshell: 
|_  (Use --script-args=ms-sql-xp-cmdshell.cmd='<CMD>' to change command.)
| ms-sql-config: 
|   192.168.224.248:49965: 
|_  ERROR: Bad username or password
|_ssl-date: 2024-04-03T04:06:05+00:00; 0s from scanner time.

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:06:34 2024 -- 1 IP address (1 host up) scanned in 85.24 seconds
