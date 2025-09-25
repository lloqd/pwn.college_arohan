# Challenge 6: listing files
Using the `ls` command to list the contents of a directory
## Solution
Invoke `ls` with `/challenge` as an argument and then invoke  `/challenge/6882-renamed-run-29865`
```
hacker@commands~listing-files:~$ ls /challenge
6882-renamed-run-29865  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/6882-renamed-run-29865
Yahaha, you found me! Here is your flag:
pwn.college{86fsDHcirV5Tx4o0v_pzbcyFjNR.QX4IDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{86fsDHcirV5Tx4o0v_pzbcyFjNR.QX4IDO0wiMwAzNzEzW}`
### Notes
- learnt about the `ls` command, which lists all files present in the directory(s) provided to it as arguments
- when no arguments are given, it defaults to the `cwd`