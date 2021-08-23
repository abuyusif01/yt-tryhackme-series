`export ip=10.10.50.184`</br> </br>

# Scanning result</br>

</br>
PORT STATE SERVICE </br>
22/tcp open ssh </br>
80/tcp open http </br>
MAC Address: 02:97:C5:68:EB:0D (Unknown)</br>
</br>
# Creds</br>
</br>
login.php --> R1ckRul3s:</br>
</br>
# gobuster</br>
</br>
`gobuster dir -u $ip -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x php,bak,zip,txt`</br>
/login.php (Status: 200)</br>
/assets (Status: 301)</br>
/portal.php (Status: 302)</br>
/robots.txt (Status: 200)</br>
/denied.php (Status: 302) </br>
/server-status (Status: 403)</br>
/clue.txt (Status: 200)</br>
</br>
# flags</br>
</br>
flag1:mr. meeseek hair </br>
flag2:1 jerry tear </br>
flag3:fleeb juice</br>
