# Challenge 4: Killing Misbehaving Processes

## Solution

```
hacker@processes~killing-misbehaving-processes:~$ ps aux | grep /challenge/decoy
root         139  0.0  0.0   5204  3520 ?        S    19:29   0:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
hacker       142  0.9  0.0  13516  9280 ?        Ss   19:29   0:00 /usr/bin/python /challenge/decoy
hacker       160  0.0  0.0 230696  2560 pts/0    S+   19:29   0:00 grep --color=auto /challenge/decoy
hacker@processes~killing-misbehaving-processes:~$ kill 142
```

```
hacker@processes~killing-misbehaving-processes:~$ /challenge/run | cat /tmp/flag_fifo
pwn.college{8C-1zueYrkZEZT8u6vOxP2c0--Z.0FNzMDOxwiMwAzNzEzW}
```

## Flag
`pwn.college{8C-1zueYrkZEZT8u6vOxP2c0--Z.0FNzMDOxwiMwAzNzEzW}`
### Notes
-