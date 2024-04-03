[*] msrpc on tcp/135

	[-] RPC Client:

		rpcclient -p 135 -U "" 192.168.224.250

[*] netbios-ssn on tcp/139

	[-] Bruteforce SMB

		crackmapexec smb 192.168.224.250 --port=139 -u "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -p "/usr/share/seclists/Passwords/darkweb2017-top100.txt"

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 139 --script="smb-vuln-* and dos" --script-args="unsafe=1" -oN "/home/kali/Documents/Relia/results/192.168.224.250/scans/tcp139/tcp_139_smb_vulnerabilities.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.250/scans/tcp139/xml/tcp_139_smb_vulnerabilities.xml" 192.168.224.250

[*] microsoft-ds on tcp/445

	[-] Bruteforce SMB

		crackmapexec smb 192.168.224.250 --port=445 -u "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -p "/usr/share/seclists/Passwords/darkweb2017-top100.txt"

	[-] Lookup SIDs

		impacket-lookupsid '[username]:[password]@192.168.224.250'

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 445 --script="smb-vuln-* and dos" --script-args="unsafe=1" -oN "/home/kali/Documents/Relia/results/192.168.224.250/scans/tcp445/tcp_445_smb_vulnerabilities.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.250/scans/tcp445/xml/tcp_445_smb_vulnerabilities.xml" 192.168.224.250

[*] ms-wbt-server on tcp/3389

	[-] Bruteforce logins:

		hydra -L "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e nsr -s 3389 -o "/home/kali/Documents/Relia/results/192.168.224.250/scans/tcp3389/tcp_3389_rdp_hydra.txt" rdp://192.168.224.250

		medusa -U "/usr/share/seclists/Usernames/cirt-default-usernames.txt" -P "/usr/share/seclists/Passwords/darkweb2017-top100.txt" -e ns -n 3389 -O "/home/kali/Documents/Relia/results/192.168.224.250/scans/tcp3389/tcp_3389_rdp_medusa.txt" -M rdp -h 192.168.224.250

[*] msrpc on tcp/49669

	[-] RPC Client:

		rpcclient -p 49669 -U "" 192.168.224.250

[*] msrpc on tcp/49670

	[-] RPC Client:

		rpcclient -p 49670 -U "" 192.168.224.250

