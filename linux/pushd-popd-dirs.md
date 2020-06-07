pushd, popd, and dirs are shell builtins which allow you manipulate the directory stack. 
This can be used to change directories but return to the directory from which you came.

pushd /home; pushd /var; pushd log
To see the stack use dirs and for easier navigation (to get the numbers of the "stack-entries" use:

dirs -v
Output:

```
me@myhost:/home$ dirs -v
 0  /home
 1  /var
 2  /tmp
```
Now utilize these numbers with cd and ~ like:

cd ~1
But these numbers are rearranged now and position "0" will change, so just pushd the directory to the top position twice (or use a dummy on position 0) like:

```
me@myhost:/home$ dirs -v
 0  /home
 1  /home
 2  /var
 3  /tmp
```
now 1..3 will keep there position

