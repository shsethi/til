arbitrary TCP and UDP connections and listens

 The nc (or netcat) utility is used for just about anything under the sun
     involving TCP or UDP.  It can open TCP connections, send UDP packets, lis-
     ten on arbitrary TCP and UDP ports, do port scanning, and deal with both
     IPv4 and IPv6.

```
# connect to udp connection on port 5501

nc -u 127.0.0.1 5501

```