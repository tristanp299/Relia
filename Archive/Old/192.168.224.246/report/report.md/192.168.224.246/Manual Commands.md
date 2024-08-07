```bash
[*] http on tcp/80

	[-] (feroxbuster) Multi-threaded recursive directory/file enumeration for web servers using various wordlists:

		feroxbuster -u http://192.168.224.246:80 -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -e -r -o /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_feroxbuster_dirbuster.txt

	[-] Credential bruteforcing commands (don't run these without modifying them):

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 80 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_auth_hydra.txt" http-get://192.168.224.246/path/to/auth/area

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 80 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_auth_medusa.txt" -M http -h 192.168.224.246 -m DIR:/path/to/auth/area

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 80 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_form_hydra.txt" http-post-form://192.168.224.246/path/to/login.php:"username=^USER^&password=^PASS^":"invalid-login-message"

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 80 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_form_medusa.txt" -M web-form -h 192.168.224.246 -m FORM:/path/to/login.php -m FORM-DATA:"post?username=&password=" -m DENY-SIGNAL:"invalid login message"

	[-] (wpscan) WordPress Security Scanner (useful if WordPress is found):

		wpscan --url http://192.168.224.246:80/ --no-update -e vp,vt,tt,cb,dbe,u,m --plugins-detection aggressive --plugins-version-detection aggressive -f cli-no-color 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_wpscan.txt"

[*] http on tcp/443

	[-] (feroxbuster) Multi-threaded recursive directory/file enumeration for web servers using various wordlists:

		feroxbuster -u https://192.168.224.246:443 -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -e -r -o /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_dirbuster.txt

	[-] Credential bruteforcing commands (don't run these without modifying them):

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 443 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_auth_hydra.txt" https-get://192.168.224.246/path/to/auth/area

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 443 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_auth_medusa.txt" -M http -h 192.168.224.246 -m DIR:/path/to/auth/area

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 443 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_form_hydra.txt" https-post-form://192.168.224.246/path/to/login.php:"username=^USER^&password=^PASS^":"invalid-login-message"

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 443 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_form_medusa.txt" -M web-form -h 192.168.224.246 -m FORM:/path/to/login.php -m FORM-DATA:"post?username=&password=" -m DENY-SIGNAL:"invalid login message"

	[-] (wpscan) WordPress Security Scanner (useful if WordPress is found):

		wpscan --url https://192.168.224.246:443/ --no-update -e vp,vt,tt,cb,dbe,u,m --plugins-detection aggressive --plugins-version-detection aggressive -f cli-no-color 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_wpscan.txt"

[*] ssh on tcp/2222

	[-] Bruteforce logins:

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 2222 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/tcp_2222_ssh_hydra.txt" ssh://192.168.224.246

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 2222 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/tcp_2222_ssh_medusa.txt" -M ssh -h 192.168.224.246

[*] https on tcp/443

	[-] (feroxbuster) Multi-threaded recursive directory/file enumeration for web servers using various wordlists:

		feroxbuster -u https://192.168.224.246:443 -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -e -r -o /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_feroxbuster_dirbuster.txt

	[-] Credential bruteforcing commands (don't run these without modifying them):

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 443 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_auth_hydra.txt" https-get://192.168.224.246/path/to/auth/area

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 443 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_auth_medusa.txt" -M http -h 192.168.224.246 -m DIR:/path/to/auth/area

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 443 -o "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_form_hydra.txt" https-post-form://192.168.224.246/path/to/login.php:"username=^USER^&password=^PASS^":"invalid-login-message"

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 443 -O "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_form_medusa.txt" -M web-form -h 192.168.224.246 -m FORM:/path/to/login.php -m FORM-DATA:"post?username=&password=" -m DENY-SIGNAL:"invalid login message"

	[-] (wpscan) WordPress Security Scanner (useful if WordPress is found):

		wpscan --url https://192.168.224.246:443/ --no-update -e vp,vt,tt,cb,dbe,u,m --plugins-detection aggressive --plugins-version-detection aggressive -f cli-no-color 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_wpscan.txt"


```