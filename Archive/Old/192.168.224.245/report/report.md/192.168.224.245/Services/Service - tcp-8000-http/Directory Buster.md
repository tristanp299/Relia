```bash
feroxbuster -u http://192.168.224.245:8000/ -t 100 -w /usr/share/seclists/Discovery/Web-Content/common.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_common.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_common.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_common.txt):

```
200      GET       24l       55w      853c http://192.168.224.245:8000/js/main.js
200      GET      146l      296w     2600c http://192.168.224.245:8000/style/style.css
200      GET        0l        0w   709931c http://192.168.224.245:8000/img/relia.png
200      GET       52l       96w     1709c http://192.168.224.245:8000/
200      GET       52l       96w     1709c http://192.168.224.245:8000/index.html
200      GET        1l        4w       38c http://192.168.224.245:8000/login

```
```bash
feroxbuster -u http://192.168.224.245:8000/ -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_directory-list-2.3-medium.txt"
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_directory-list-2.3-medium.txt](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_directory-list-2.3-medium.txt):

```
200      GET        1l        4w       38c http://192.168.224.245:8000/login
200      GET      146l      296w     2600c http://192.168.224.245:8000/style/style.css
200      GET       24l       55w      853c http://192.168.224.245:8000/js/main.js
200      GET       52l       96w     1709c http://192.168.224.245:8000/index.html
200      GET     1876l    13702w  1302133c http://192.168.224.245:8000/img/relia.png
200      GET       52l       96w     1709c http://192.168.224.245:8000/

```
