arbitrary TCP and UDP connections and listens

 The nc (or netcat) utility is used for just about anything under the sun
     involving TCP or UDP.  It can open TCP connections, send UDP packets, lis-
     ten on arbitrary TCP and UDP ports, do port scanning, and deal with both
     IPv4 and IPv6.

```
# connect to udp connection on port 5501

nc -u 127.0.0.1 5501

```


----

After a listening UDP port got it's first packet, it will only accept additional input if it comes from the same sending port.

If you want to connect to same udp connection again and again you need to specify the source port

```
nc -u 127.0.0.1 1299 -p 2000
```

https://serverfault.com/questions/773110/make-netcat-listen-for-multiple-udp-packets
