```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 443 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/xml/tcp_443_https_nmap.xml" 192.168.224.245
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:58:59 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 443 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/xml/tcp_443_https_nmap.xml 192.168.224.245
Nmap scan report for 192.168.224.245
Host is up, received user-set.
Scanned at 2024-04-02 20:58:59 PDT for 1s

PORT    STATE    SERVICE REASON      VERSION
443/tcp filtered https   no-response

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:59:00 2024 -- 1 IP address (1 host up) scanned in 1.45 seconds

```
