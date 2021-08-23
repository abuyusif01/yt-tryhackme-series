`export ip=10.10.50.184`

# Scanning result

PORT STATE SERVICE 22/tcp open ssh 80/tcp open http MAC Address:
02:97:C5:68:EB:0D (Unknown)

# Creds

login.php --> R1ckRul3s:

# gobuster

`gobuster dir -u $ip -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x php,bak,zip,txt`
/login.php (Status: 200) /assets (Status: 301) /portal.php (Status: 302)
/robots.txt (Status: 200) /denied.php (Status: 302) /server-status (Status: 403)
/clue.txt (Status: 200)

# flags

flag1:mr. meeseek hair flag2:1 jerry tear flag3:fleeb juice
