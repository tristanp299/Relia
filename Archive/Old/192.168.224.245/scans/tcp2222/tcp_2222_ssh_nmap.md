# Nmap 7.94SVN scan initiated Tue Apr  2 20:59:14 2024 as: nmap -vv --reason -Pn -T4 -T4 --min-rate=500 -sV -p 2222 --script=banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods -oN /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp2222/tcp_2222_ssh_nmap.txt -oX /home/kali/Documents/Relia/results/192.168.224.245/scans/tcp2222/xml/tcp_2222_ssh_nmap.xml 192.168.224.245
Nmap scan report for 192.168.224.245
Host is up, received user-set (0.073s latency).
Scanned at 2024-04-02 20:59:14 PDT for 8s

PORT     STATE SERVICE REASON         VERSION
2222/tcp open  ssh     syn-ack ttl 61 OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
| ssh2-enum-algos: 
|   kex_algorithms: (9)
|       curve25519-sha256
|       curve25519-sha256@libssh.org
|       ecdh-sha2-nistp256
|       ecdh-sha2-nistp384
|       ecdh-sha2-nistp521
|       diffie-hellman-group-exchange-sha256
|       diffie-hellman-group16-sha512
|       diffie-hellman-group18-sha512
|       diffie-hellman-group14-sha256
|   server_host_key_algorithms: (5)
|       rsa-sha2-512
|       rsa-sha2-256
|       ssh-rsa
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
| ssh-auth-methods: 
|   Supported authentication methods: 
|_    publickey
| ssh-hostkey: 
|   3072 30:0c:6c:9b:ac:07:47:5e:df:6d:ff:38:63:38:2a:fd (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCkRPaVboTfq+VZYyf1bsUlg+WZrPP1F6fRrA0TNkHmamfuFAhW9XfCiuh2GOnSkNeGUXLcMAgMtbki6uj4l6vTw5/pqM/jBz00be6Ty+g0CDz9gmb+p0iX+8vCeG6aB0vea9bvkjaABticCS1CmUEbfEe/jCn/11c4NmHleCFfVxE8PBRE2OyVWlFQkkcB74O0FS4AOfbnrAx3pAF4rcd7XsTgi4V1e/sKZ8RIcTlueVdnzZEMcpLeZXUR1cXsJ9zwklFLuMWuUjonYC7BFvT+Bf81jlO1/e9B0RxfalfCfeUthSoa2VGwpfvesCdHl0exvy1PXaeR2XUX5ZJ0jmoP7cvj1rb+ZrnUU/Sie0qpVklHpkjggz0li7Mk4h/CI+est9oeHP+UXVv+Xl/jpnXz/RX/1y03wkTe9Pygxo3NsLdrs22/UCQ5GZ5x78UJQBXCCI93KHY1BG28B9V8xT9PGmpFDgjnF3pFuZoMevmeHSVNBlNQV42/qFCJr48XbAM=
|   256 f3:a9:70:76:c8:d4:c4:17:f4:39:1f:be:58:9d:1f:a5 (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBK6SiUV5zqxqNJ9a/p9l+VpxxqiXnYri40OjXMExS/tP0EbTAEpojn4uXKOgR3oEaMmQVmI9QLPTehCFLNJ3iJo=
|   256 21:a0:79:82:2d:e6:2a:76:11:24:2f:7e:2e:a8:c7:83 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIJ9WPZpl/+VGWtnGi3tQSn1u5FAiDr9bKTV2xCUqje/c
|_banner: SSH-2.0-OpenSSH_8.2p1 Ubuntu-4ubuntu0.5
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Apr  2 20:59:22 2024 -- 1 IP address (1 host up) scanned in 8.54 seconds
