[*] http on tcp/80

	[-] (feroxbuster) Multi-threaded recursive directory/file enumeration for web servers using various wordlists:

		feroxbuster -u http://192.168.224.247:80 -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -e -r -o /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_feroxbuster_dirbuster.txt

	[-] Credential bruteforcing commands (don't run these without modifying them):

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 80 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_auth_hydra.txt" http-get://192.168.224.247/path/to/auth/area

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 80 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_auth_medusa.txt" -M http -h 192.168.224.247 -m DIR:/path/to/auth/area

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 80 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_form_hydra.txt" http-post-form://192.168.224.247/path/to/login.php:"username=^USER^&password=^PASS^":"invalid-login-message"

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 80 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_form_medusa.txt" -M web-form -h 192.168.224.247 -m FORM:/path/to/login.php -m FORM-DATA:"post?username=&password=" -m DENY-SIGNAL:"invalid login message"

	[-] (wpscan) WordPress Security Scanner (useful if WordPress is found):

		wpscan --url http://192.168.224.247:80/ --no-update -e vp,vt,tt,cb,dbe,u,m --plugins-detection aggressive --plugins-version-detection aggressive -f cli-no-color 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp80/tcp_80_http_wpscan.txt"

[*] msrpc on tcp/135

	[-] RPC Client:

		rpcclient -p 135 -U "" 192.168.224.247

[*] netbios-ssn on tcp/139

	[-] Bruteforce SMB

		crackmapexec smb 192.168.224.247 --port=139 -u "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -p "/usr/share/seclists/Passwords/darkweb2017-top100.txt"

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 139 --script="smb-vuln-* and dos" --script-args="unsafe=1" -oN "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp139/tcp_139_smb_vulnerabilities.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp139/xml/tcp_139_smb_vulnerabilities.xml" 192.168.224.247

[*] http on tcp/443

	[-] (feroxbuster) Multi-threaded recursive directory/file enumeration for web servers using various wordlists:

		feroxbuster -u https://192.168.224.247:443 -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -e -r -o /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp443/tcp_443_https_feroxbuster_dirbuster.txt

	[-] Credential bruteforcing commands (don't run these without modifying them):

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 443 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp443/tcp_443_https_auth_hydra.txt" https-get://192.168.224.247/path/to/auth/area

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 443 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp443/tcp_443_https_auth_medusa.txt" -M http -h 192.168.224.247 -m DIR:/path/to/auth/area

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 443 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp443/tcp_443_https_form_hydra.txt" https-post-form://192.168.224.247/path/to/login.php:"username=^USER^&password=^PASS^":"invalid-login-message"

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 443 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp443/tcp_443_https_form_medusa.txt" -M web-form -h 192.168.224.247 -m FORM:/path/to/login.php -m FORM-DATA:"post?username=&password=" -m DENY-SIGNAL:"invalid login message"

	[-] (wpscan) WordPress Security Scanner (useful if WordPress is found):

		wpscan --url https://192.168.224.247:443/ --no-update -e vp,vt,tt,cb,dbe,u,m --plugins-detection aggressive --plugins-version-detection aggressive -f cli-no-color 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp443/tcp_443_https_wpscan.txt"

[*] microsoft-ds on tcp/445

	[-] Bruteforce SMB

		crackmapexec smb 192.168.224.247 --port=445 -u "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -p "/usr/share/seclists/Passwords/darkweb2017-top100.txt"

	[-] Lookup SIDs

		impacket-lookupsid '[username]:[password]@192.168.224.247'

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 445 --script="smb-vuln-* and dos" --script-args="unsafe=1" -oN "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp445/tcp_445_smb_vulnerabilities.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp445/xml/tcp_445_smb_vulnerabilities.xml" 192.168.224.247

[*] ms-wbt-server on tcp/3389

	[-] Bruteforce logins:

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 3389 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp3389/tcp_3389_rdp_hydra.txt" rdp://192.168.224.247

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 3389 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp3389/tcp_3389_rdp_medusa.txt" -M rdp -h 192.168.224.247

[*] wsman on tcp/5985

	[-] Bruteforce logins:

		crackmapexec winrm 192.168.224.247 -d '<domain>' -u '/usr/share/seclists/Usernames/cirt-default-usernames.txt' -p '/usr/share/seclists/Passwords/darkweb2017-top100.txt'

	[-] Check login (requires credentials):

		crackmapexec winrm 192.168.224.247 -d '<domain>' -u '<username>' -p '<password>'

	[-] Evil WinRM (gem install evil-winrm):

		evil-winrm -u '<user>' -p '<password>' -i 192.168.224.247

		evil-winrm -u '<user>' -H '<hash>' -i 192.168.224.247

[*] ftp on tcp/14020

	[-] Bruteforce logins:

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 14020 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp14020/tcp_14020_ftp_hydra.txt" ftp://192.168.224.247

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 14020 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp14020/tcp_14020_ftp_medusa.txt" -M ftp -h 192.168.224.247

[*] http on tcp/47001

	[-] (feroxbuster) Multi-threaded recursive directory/file enumeration for web servers using various wordlists:

		feroxbuster -u http://192.168.224.247:47001 -t 100 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x "txt,html,php,asp,aspx,jsp,xml,config,bak" -v -k -n -e -r -o /home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_feroxbuster_dirbuster.txt

	[-] Credential bruteforcing commands (don't run these without modifying them):

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 47001 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_auth_hydra.txt" http-get://192.168.224.247/path/to/auth/area

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 47001 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_auth_medusa.txt" -M http -h 192.168.224.247 -m DIR:/path/to/auth/area

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 47001 -o "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_form_hydra.txt" http-post-form://192.168.224.247/path/to/login.php:"username=^USER^&password=^PASS^":"invalid-login-message"

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 47001 -O "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_form_medusa.txt" -M web-form -h 192.168.224.247 -m FORM:/path/to/login.php -m FORM-DATA:"post?username=&password=" -m DENY-SIGNAL:"invalid login message"

	[-] Bruteforce logins:

		crackmapexec winrm 192.168.224.247 -d '<domain>' -u '/usr/share/seclists/Usernames/cirt-default-usernames.txt' -p '/usr/share/seclists/Passwords/darkweb2017-top100.txt'

	[-] Check login (requires credentials):

		crackmapexec winrm 192.168.224.247 -d '<domain>' -u '<username>' -p '<password>'

	[-] Evil WinRM (gem install evil-winrm):

		evil-winrm -u '<user>' -p '<password>' -i 192.168.224.247

		evil-winrm -u '<user>' -H '<hash>' -i 192.168.224.247

	[-] (wpscan) WordPress Security Scanner (useful if WordPress is found):

		wpscan --url http://192.168.224.247:47001/ --no-update -e vp,vt,tt,cb,dbe,u,m --plugins-detection aggressive --plugins-version-detection aggressive -f cli-no-color 2>&1 | tee "/home/kali/Documents/Relia/results/192.168.224.247/scans/tcp47001/tcp_47001_http_wpscan.txt"

