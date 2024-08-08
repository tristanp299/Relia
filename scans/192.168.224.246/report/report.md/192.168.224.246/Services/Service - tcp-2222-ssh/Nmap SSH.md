```bash
nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 2222 --script="banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods" -oN "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/tcp_2222_ssh_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/xml/tcp_2222_ssh_nmap.xml" 192.168.224.246
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/tcp_2222_ssh_nmap.txt](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/tcp_2222_ssh_nmap.txt):

```
# Nmap 7.94SVN scan initiated Tue Apr  2 20:57:13 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 2222 --script=banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods -oN /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/tcp_2222_ssh_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp2222/xml/tcp_2222_ssh_nmap.xml 192.168.224.246
Nmap scan report for 192.168.224.246
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 20:57:13 PDT for 3s

PORT     STATE SERVICE REASON         VERSION
2222/tcp open  ssh     syn-ack ttl 61 OpenSSH 8.9p1 Ubuntu 3 (Ubuntu Linux; protocol 2.0)
| ssh-auth-methods: 
|   Supported authentication methods: 
|_    publickey
|_banner: SSH-2.0-OpenSSH_8.9p1 Ubuntu-3
| ssh2-enum-algos: 
|   kex_algorithms: (10)
|       curve25519-sha256
|       curve25519-sha256@libssh.org
|       ecdh-sha2-nistp256
|       ecdh-sha2-nistp384
|       ecdh-sha2-nistp521
|       sntrup761x25519-sha512@openssh.com
|       diffie-hellman-group-exchange-sha256
|       diffie-hellman-group16-sha512
|       diffie-hellman-group18-sha512
|       diffie-hellman-group14-sha256
|   server_host_key_algorithms: (4)
|       rsa-sha2-512
|       rsa-sha2-256
|       ecdsa-sha2-nistp256
|       ssh-ed25519
|   encryption_algorithms: (6)
|       chacha20-poly1305@openssh.com
|       aes128-ctr
|       aes192-ctr
|       aes256-ctr
|       aes128-gcm@openssh.com
|       aes256-gcm@openssh.com
|   mac_algorithms: (10)
|       umac-64-etm@openssh.com
|       umac-128-etm@openssh.com
|       hmac-sha2-256-etm@openssh.com
|       hmac-sha2-512-etm@openssh.com
|       hmac-sha1-etm@openssh.com
|       umac-64@openssh.com
|       umac-128@openssh.com
|       hmac-sha2-256
|       hmac-sha2-512
|       hmac-sha1
|   compression_algorithms: (2)
|       none
|_      zlib@openssh.com
| ssh-hostkey: 
|   256 42:2d:8d:48:ad:10:dd:ff:70:25:8b:46:2e:5c:ff:1d (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBEpVNr/0MSfOq95rNQVnUXG+NF7yHDkPeFEXylLHxnZSqLAEqWi+z67gxHF0QVSjtaeEVbOnind7C3LKLGe1b8g=
|   256 aa:4a:c3:27:b1:19:30:d7:63:91:96:ae:63:3c:07:dc (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIFcUmhqn+iJNZi0wDswh/Jusg6ZX0SGGoKcsNCB69vQA
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:57:16 2024 -- 1 IP address (1 host up) scanned in 2.77 seconds

```
