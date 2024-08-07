```bash
feroxbuster -u http://192.168.224.246:80/ -t 100 -w /usr/share/seclists/Discovery/Web-Content/common.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_common.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_common.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_common.txt):

```
200      GET        5l     1434w    97163c http://192.168.224.246/js/jquery-1.12.4.min.js
200      GET       52l      110w     1516c http://192.168.224.246/
200      GET       16l       58w      950c http://192.168.224.246/css/
200      GET        1l        3w       47c http://192.168.224.246/submit/

```
```bash
feroxbuster -u http://192.168.224.246:80/ -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_directory-list-2.3-medium.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_directory-list-2.3-medium.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_directory-list-2.3-medium.txt):

```
200      GET       22l       77w      820c http://192.168.224.246/js/scripts.js
200      GET       52l      110w     1516c http://192.168.224.246/index.php
200      GET        6l     1429w   121200c http://192.168.224.246/css/bootstrap.min.css
200      GET        5l     1434w    97163c http://192.168.224.246/js/jquery-1.12.4.min.js
200      GET       52l      110w     1516c http://192.168.224.246/
200      GET        1l        3w       47c http://192.168.224.246/submit/
200      GET       16l       58w      950c http://192.168.224.246/css/
200      GET       17l       69w     1152c http://192.168.224.246/js/

```
