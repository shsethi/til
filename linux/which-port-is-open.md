### What ports are open on your computer

linux
```sh
$ 
netstat -tulpn  # netstat tells you 
```

mac
```sh
$ 

lsof -PiTCP -sTCP:LISTEN

$
netstat  -anv -p tcp -f inet | grep 5432
