# Challenge 2: Killing Processes

## Solution

```
hacker@processes~killing-processes:~$ ps aux | grep challenge
root         135  0.0  0.0   5204  3520 ?        S    19:16   0:00 su -c /challenge/.launcher hacker
hacker       136  0.0  0.0 231576  3520 ?        Ss   19:16   0:00 /challenge/dont_run
hacker       155  0.0  0.0 230696  2560 pts/0    S+   19:16   0:00 grep --color=auto challenge
hacker@processes~killing-processes:~$ kill 136
```

```
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{QZJbX2D-uiJspuye5e96Nad47wP.QXyQDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{QZJbX2D-uiJspuye5e96Nad47wP.QXyQDO0wiMwAzNzEzW}`
### Notes
-