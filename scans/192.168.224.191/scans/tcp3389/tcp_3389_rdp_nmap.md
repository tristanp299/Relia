# Nmap 7.94SVN scan initiated Tue Apr  2 21:09:45 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 3389 "--script=banner,(rdp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.191/scans/tcp3389/tcp_3389_rdp_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.191/scans/tcp3389/xml/tcp_3389_rdp_nmap.xml 192.168.224.191
Nmap scan report for 192.168.224.191
Host is up, received user-set (0.078s latency).
Scanned at 2024-04-02 21:09:45 PDT for 53s

PORT     STATE SERVICE       REASON          VERSION
3389/tcp open  ms-wbt-server syn-ack ttl 125 Microsoft Terminal Services
| rdp-ntlm-info: 
|   Target_Name: RELIA
|   NetBIOS_Domain_Name: RELIA
|   NetBIOS_Computer_Name: LOGIN
|   DNS_Domain_Name: relia.com
|   DNS_Computer_Name: login.relia.com
|   DNS_Tree_Name: relia.com
|   Product_Version: 10.0.20348
|_  System_Time: 2024-04-03T04:09:54+00:00
|_ssl-date: 2024-04-03T04:10:12+00:00; -1s from scanner time.
| ssl-cert: Subject: commonName=login.relia.com
| Issuer: commonName=login.relia.com
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-04-02T03:51:24
| Not valid after:  2024-10-02T03:51:24
| MD5:   a11e:74d0:3e26:9798:2cd2:23b4:042e:7ea8
| SHA-1: 7baa:db80:8004:6091:c748:8c30:31ec:b549:df13:cbc4
| -----BEGIN CERTIFICATE-----
| MIIC4jCCAcqgAwIBAgIQdtruqDnQ7o1IYp27loS04zANBgkqhkiG9w0BAQsFADAa
| MRgwFgYDVQQDEw9sb2dpbi5yZWxpYS5jb20wHhcNMjQwNDAyMDM1MTI0WhcNMjQx
| MDAyMDM1MTI0WjAaMRgwFgYDVQQDEw9sb2dpbi5yZWxpYS5jb20wggEiMA0GCSqG
| SIb3DQEBAQUAA4IBDwAwggEKAoIBAQC8DfO9QNR6IxkrhxgIcZJlF9X079dzXb6N
| Q8qp64tpPKS27rkJXJPbkqNL+46rx10B9pZZ+WH0bo6AEzxfOmlckq9Fe6cyhC6m
| vhJcO4z58Rw9zf80K9LgSDLIE6+QplWGyTMuI9kSAyfLWlUxse16YCuDqlg+H+LT
| XHrGkBPsuIrsl+MRWcGJzl7DhhAVCuoN+MW9TgEGbzyos8Sk+KrmnSADFmZB4cy6
| QfhQJQ6NpZGrc6piG/88fLikkfHg39xjxulOStJBiTqAkTjTonrCmTaCkPKn/m3d
| 5bSkGasE85nDV7VK0DHBdVyVPNbnJzbseEGNEEWj71yW6EigR5/9AgMBAAGjJDAi
| MBMGA1UdJQQMMAoGCCsGAQUFBwMBMAsGA1UdDwQEAwIEMDANBgkqhkiG9w0BAQsF
| AAOCAQEACXRXVXR8GGwZfbEoeWtaYarPb3tckZSBigGZQPztq86zO4qZELPiKxsp
| s0YCWsbkoQxS9FrZNhHPgGTeMRbhVPo2X88imYAiRArPl8MRMuVnerfgrMl95J+I
| j4wWtE2MquG6YiReFaHnQXaOxn6x4ePSWz8qooQ6+Yv3yzFgo4uKTdiTeYzNrP66
| 1BeeUNlgmnOuB6jkA4uTz94wvL56W+gQho+Y7Y4xPHkfZ7ec/Q7jBiNgquC/2PEN
| zcOLE6hcvFvV3L+RvvuNsslXmdXUSDW8YUx1F7s1id1jBFPqLnXC/fpK9BkG8Nr1
| Al1W/WvjrrFH0KMIayCzSTLjzPBxNw==
|_-----END CERTIFICATE-----
| rdp-enum-encryption: 
|   Security layer
|     CredSSP (NLA): SUCCESS
|     CredSSP with Early User Auth: SUCCESS
|_    RDSTLS: SUCCESS
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 21:10:38 2024 -- 1 IP address (1 host up) scanned in 52.96 seconds
