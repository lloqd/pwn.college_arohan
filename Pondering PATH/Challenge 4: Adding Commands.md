# Challenge 4: Adding Commands
"Creating" a _shell_ command using _bash_ scripts and `PATH`
## Solution
Invoke `which cat` to get the path for `cat` since we will wipe `PATH` soon, and create a script `win` using `nano`
```
hacker@path~adding-commands:~$ which cat
/run/dojo/bin/cat
hacker@path~adding-commands:~$ nano win
```
The script:
```
#!/bin/bash
/run/dojo/bin/cat /flag
```
Now, we make `win` an executable using `chmod a+x`, set `PATH` to be `~/` and invoke `/challenge/run`
```
hacker@path~adding-commands:~$ chmod a+x win
hacker@path~adding-commands:~$ PATH="~/"
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{sXW08a66eesdxzSbnrHvDdjQpeH.QX2cjM1wiMwAzNzEzW}
```
## Flag
`pwn.college{sXW08a66eesdxzSbnrHvDdjQpeH.QX2cjM1wiMwAzNzEzW}`