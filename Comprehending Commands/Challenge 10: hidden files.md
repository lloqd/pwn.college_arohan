# Challenge 10: hidden files
Using `ls -a` to list hidden files in a directory
## Solution
Invoke `ls` with `-a` as an argument to list the _hidden_ files in the directory, i.e. `.flag-19137286318198` in this case, which we will use as an argument for `cat`
```
hacker@commands~hidden-files:~$ ls -a /
.  ..  .dockerenv  .flag-19137286318198  bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~hidden-files:~$ cat /.flag-19137286318198
pwn.college{4r7SjhIv6mA50SGKytmi5Y-079I.QXwUDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{4r7SjhIv6mA50SGKytmi5Y-079I.QXwUDO0wiMwAzNzEzW}`
### Notes
- learnt about the Linux convention for hidden files/directories, i.e. the `.` prefix, which prevents them from showing up in `ls` and similar contexts
- to list hidden files with `ls`, the `-a` argument is used 