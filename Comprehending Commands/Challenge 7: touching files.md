# Challenge 7: touching files
Using `touch` to create a file at a specified path
## Solution
Invoke `touch` to create files at `/tmp/pwn` and `/tmp/college`, then run `/challenge/run`
```
hacker@commands~touching-files:~$ touch /tmp/pwn
hacker@commands~touching-files:~$ touch /tmp/college
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{UEhV-xr1u0Oj4COQqogFNRP96gI.QXwMDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{UEhV-xr1u0Oj4COQqogFNRP96gI.QXwMDO0wiMwAzNzEzW}`
### Notes
- learnt about the `touch` command, which can create a new, blank file at the path provided to it