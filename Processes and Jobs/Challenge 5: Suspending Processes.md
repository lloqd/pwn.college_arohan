# Challenge 5: Suspending Processses

## Solution

```
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         138     129  0 08:45 pts/0    00:00:00 bash /challenge/run
root         140     138  0 08:45 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
```

```
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         138     129  0 08:45 pts/0    00:00:00 bash /challenge/run
root         145     129  0 08:45 pts/0    00:00:00 bash /challenge/run
root         147     145  0 08:45 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{YjSfA-2AveP7_wUPaSQdR1l3ZJK.QX1QDO0wiMwAzNzEzW}
```
## Flag
`pwn.college{YjSfA-2AveP7_wUPaSQdR1l3ZJK.QX1QDO0wiMwAzNzEzW}`
### Notes
-