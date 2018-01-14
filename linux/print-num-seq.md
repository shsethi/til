### seq
* print num 1 to 100
```
seq 1 100
```
* with space (" ") as seprater
```
seq -s " " 1 100
```
* with a increment of 5
```
seq -s " " 1 5 100
```

### jot
* print 10 random numbers
 ```
 jot -r 10
 ```

 * print 20 random 8-letter strings

 ```
 jot -r -c 160 a z | rs -g 0 8

