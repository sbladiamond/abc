### Links
* [Практические советы, примеры и туннели SSH](https://habr.com/en/post/435546/)
* https://russianblogs.com/article/3838446135/

### Resource
* https://hackertarget.com/
* https://www.linuxhowto.net/install-and-configure-vnc-on-ubuntu-20-04/

### Cheatsheet
* [ip-command-cheat-sheet.pdf](https://github.com/sbladiamond/abc/files/7126931/ip-command-cheat-sheet.pdf)


### Commix
https://codeby.net/threads/commix-prostymi-slovami.67620/
https://github.com/sbladiamond/abc/blob/main/eu-15-Stasinopoulos-Commix-Detecting-And-Exploiting-Command-Injection-Flaws.pdf


### HOWTO
https://www.postexplo.com/forum/ids-ips/network-based/764-ids-evasion-techniques-using-url-encoding


### DOCKER-COMPOSE
Install oneliner
```
curl -L "https://github.com/docker/compose/releases/download/`curl -fsSLI -o /dev/null -w %{url_effective} https://github.com/docker/compose/releases/latest | sed 's#.*tag/##g' && echo`/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose && chmod +x /usr/local/bin/docker-compose
```
