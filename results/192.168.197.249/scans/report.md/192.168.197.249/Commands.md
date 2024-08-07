```bash
nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sV -sC --version-all -A --osscan-guess -oN "/home/kali/Documents/Relia/results/192.168.197.249/scans/_quick_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.197.249/scans/xml/_quick_tcp_nmap.xml" 192.168.197.249

nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/kali/Documents/Relia/results/192.168.197.249/scans/_full_tcp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.197.249/scans/xml/_full_tcp_nmap.xml" 192.168.197.249

nmap -vv --reason -Pn -T4 -T3 --min-rate=500 -sU -A --top-ports 100 -oN "/home/kali/Documents/Relia/results/192.168.197.249/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/Relia/results/192.168.197.249/scans/xml/_top_100_udp_nmap.xml" 192.168.197.249


```