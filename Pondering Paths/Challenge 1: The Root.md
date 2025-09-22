# Challenge 1: The Root
Invoking a program using it's path on the CLI

## Solution
Navigate to the `root` directory using the `cd` command and execute the `pwn` program
```
hacker@paths~the-root:~$ cd /
hacker@paths~the-root:/$ ls -a
.  ..  .dockerenv  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  pwn  root  run  sbin  srv  sys  tmp  usr  var
hacker@paths~the-root:/$ /pwn
BOOM!!!
Here is your flag:
pwn.college{QEkcL9fEO52mHR0jUPENJIBi-RP.QX4cTO0wiMwAzNzEzW}
```

## Flag
`pwn.college{QEkcL9fEO52mHR0jUPENJIBi-RP.QX4cTO0wiMwAzNzEzW}`
