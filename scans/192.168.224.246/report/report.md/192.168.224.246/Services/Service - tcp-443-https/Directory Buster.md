```bash
feroxbuster -u https://192.168.224.246:443/ -t 100 -w /usr/share/seclists/Discovery/Web-Content/common.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_common.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_common.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_common.txt):

```
200      GET       22l       77w      820c https://192.168.224.246/js/scripts.js
200      GET        6l     1429w   121200c https://192.168.224.246/css/bootstrap.min.css
200      GET        5l     1434w    97163c https://192.168.224.246/js/jquery-1.12.4.min.js
200      GET       52l      110w     1516c https://192.168.224.246/
200      GET       16l       58w      951c https://192.168.224.246/css/
200      GET       94l      534w    42816c https://192.168.224.246/fonts/glyphicons-halflings-regular.woff
200      GET       16l       60w      990c https://192.168.224.246/fonts/
200      GET       52l      110w     1516c https://192.168.224.246/index.php
200      GET       17l       69w     1153c https://192.168.224.246/js/
200      GET        1l        3w       47c https://192.168.224.246/submit/

```
```bash
feroxbuster -u https://192.168.224.246:443/ -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_directory-list-2.3-medium.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_directory-list-2.3-medium.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_directory-list-2.3-medium.txt):

```
200      GET       22l       77w      820c https://192.168.224.246/js/scripts.js
200      GET       52l      110w     1516c https://192.168.224.246/index.php
200      GET        1l        3w       47c https://192.168.224.246/submit/
200      GET        6l     1429w   121200c https://192.168.224.246/css/bootstrap.min.css
200      GET        5l     1434w    97163c https://192.168.224.246/js/jquery-1.12.4.min.js
200      GET       52l      110w     1516c https://192.168.224.246/
200      GET       16l       58w      951c https://192.168.224.246/css/
200      GET       17l       69w     1153c https://192.168.224.246/js/
200      GET       94l      534w    42816c https://192.168.224.246/fonts/glyphicons-halflings-regular.woff
200      GET       16l       60w      990c https://192.168.224.246/fonts/
200      GET       22l       77w      820c https://192.168.224.246/js/scripts.js
200      GET        6l     1429w   121200c https://192.168.224.246/css/bootstrap.min.css
200      GET       52l      110w     1516c https://192.168.224.246/index.php
200      GET        5l     1434w    97163c https://192.168.224.246/js/jquery-1.12.4.min.js
200      GET       52l      110w     1516c https://192.168.224.246/
200      GET        1l        3w       47c https://192.168.224.246/submit/
200      GET       16l       58w      951c https://192.168.224.246/css/
200      GET       17l       69w     1153c https://192.168.224.246/js/
200      GET       94l      534w    42816c https://192.168.224.246/fonts/glyphicons-halflings-regular.woff
200      GET       16l       60w      990c https://192.168.224.246/fonts/

```
