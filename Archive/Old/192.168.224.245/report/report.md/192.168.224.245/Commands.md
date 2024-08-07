```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/_quick_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/xml/_quick_tcp_nmap.xml" 192.168.224.245

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/_full_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/xml/_full_tcp_nmap.xml" 192.168.224.245

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sU -A --top-ports 100 -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/xml/_top_100_udp_nmap.xml" 192.168.224.245

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 21 --script="banner,(ftp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp21/tcp_21_ftp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp21/xml/tcp_21_ftp_nmap.xml" 192.168.224.245

feroxbuster -u http://192.168.224.245:80/ -t 100 -w /usr/share/seclists/Discovery/Web-Content/common.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_feroxbuster_common.txt"

curl -sSikf http://192.168.224.245:80/.well-known/security.txt

curl -sSikf http://192.168.224.245:80/robots.txt

curl -sSik http://192.168.224.245:80/

nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://192.168.224.245:80 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_nikto.txt"

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 80 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/xml/tcp_80_http_nmap.xml" 192.168.224.245

whatweb --color=never --no-errors -a 3 -v http://192.168.224.245:80 2>&1

wkhtmltoimage --format png http://192.168.224.245:80/ /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_screenshot.png

feroxbuster -u https://192.168.224.245:443/ -t 100 -w /usr/share/seclists/Discovery/Web-Content/common.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_feroxbuster_common.txt"

curl -sSikf https://192.168.224.245:443/.well-known/security.txt

curl -sSikf https://192.168.224.245:443/robots.txt

curl -sSik https://192.168.224.245:443/

nikto -ask=no -Tuning=x4567890ac -nointeractive -host https://192.168.224.245:443 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_nikto.txt"

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 443 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/xml/tcp_443_https_nmap.xml" 192.168.224.245

sslscan --show-certificate --no-colour 192.168.224.245:443 2>&1

whatweb --color=never --no-errors -a 3 -v https://192.168.224.245:443 2>&1

wkhtmltoimage --format png https://192.168.224.245:443/ /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_screenshot.png

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 2222 --script="banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp2222/tcp_2222_ssh_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp2222/xml/tcp_2222_ssh_nmap.xml" 192.168.224.245

feroxbuster -u http://192.168.224.245:8000/ -t 100 -w /usr/share/seclists/Discovery/Web-Content/common.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_common.txt"

curl -sSikf http://192.168.224.245:8000/.well-known/security.txt

curl -sSikf http://192.168.224.245:8000/robots.txt

curl -sSik http://192.168.224.245:8000/

nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://192.168.224.245:8000 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nikto.txt"

nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 8000 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/xml/tcp_8000_http_nmap.xml" 192.168.224.245

whatweb --color=never --no-errors -a 3 -v http://192.168.224.245:8000 2>&1

wkhtmltoimage --format png http://192.168.224.245:8000/ /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_screenshot.png

feroxbuster -u https://192.168.224.245:443/ -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp443/tcp_443_https_feroxbuster_directory-list-2.3-medium.txt"

feroxbuster -u http://192.168.224.245:80/ -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp80/tcp_80_http_feroxbuster_directory-list-2.3-medium.txt"

feroxbuster -u http://192.168.224.245:8000/ -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -q -e -r -o "/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_feroxbuster_directory-list-2.3-medium.txt"


```