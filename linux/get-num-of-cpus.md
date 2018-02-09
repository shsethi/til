```
$ lscpu
```

CPUs = Threads per core X cores per socket X sockets

output:
```
CPU(s):                16   
Thread(s) per core:    2 --> (Hyperthreading)  
Core(s) per socket:    4  
Socket(s):             2 --> (physical slot on the motherboard into which a chip is inserted)  
```


**lscpu**  gathers  CPU  architecture  information from sysfs and /proc/cpuinfo.The command output can be optimized for parsing or for easy readability by humans.The  information includes,  for example, the number of CPUs, threads, cores, sockets, an Non-Uniform Mem‐ ory Access (NUMA) nodes.  There is also information about the CPU caches an cache  sharing, family, model, bogoMIPS, byte order, and stepping.

