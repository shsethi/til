### What ports are open on your computer TCP and UDP

linux
```sh
$ 
sudo netstat -tulpn  # netstat tells you 
```

mac
```sh
$ 

lsof -PiTCP -sTCP:LISTEN

$
netstat  -anv -p tcp -f inet | grep 5432

```

---
### What unix socket  are open 

linux
```sh
$ 
sudo sudo netstat -lp -x
```
