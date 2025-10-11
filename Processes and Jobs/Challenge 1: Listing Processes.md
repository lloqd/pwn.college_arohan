# Challenge 1: Listing Processes
Listing running processes using the `ps` command
## Solution
We run `ps aux` to get a list of all the running processes
```
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.2  0.0   1056   640 ?        Ss   19:13   0:00 /sbin/docker-init -- /nix/v
root           7  0.1  0.0 231708  2560 ?        S    19:13   0:00 /run/dojo/bin/sleep 6h
root         132  0.0  0.0   4132  2560 ?        S    19:13   0:00 /challenge/27275-run-20517
root         135  0.0  0.0   2744  1280 ?        S    19:13   0:00 sleep 6h
hacker       137  2.0  0.0 231576  3520 pts/0    Ss   19:13   0:00 /nix/store/0nxvi9r5ymdlr2p2
hacker       143  0.4  0.0 231940  4160 pts/0    S    19:13   0:00 /run/dojo/bin/bash --login
hacker       152  0.0  0.0 233600  3840 pts/0    R+   19:13   0:00 ps aux
```
Now, we run the renamed program `/challenge/27275-run-20517`
```
hacker@processes~listing-processes:~$ /challenge/27275-run-20517
Yahaha, you found me! Here is your flag:
pwn.college{A-g2dgaYyqyq4kjwXOtCEYHCPun.QX4MDO0wiMwAzNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```
## Flag
`pwn.college{A-g2dgaYyqyq4kjwXOtCEYHCPun.QX4MDO0wiMwAzNzEzW}`
### Notes
-