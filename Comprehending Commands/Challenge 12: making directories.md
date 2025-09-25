# Challenge 12: making directories
Using the `mkdir` command to create a directory at a specified path
## Solution
Invoke `mkdir` with `/tmp/pwn` and `/tmp/college` as arguments to create directories at those paths, then execute `/challenge/run`
```
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ touch /tmp/pwn/college
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{IOVrz6EBS0VQfPvyYrNumWdCMmK.QXxMDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{IOVrz6EBS0VQfPvyYrNumWdCMmK.QXxMDO0wiMwAzNzEzW}`
### Notes
- learnt about the `mkdir` command, which can create a directory at the path specified to it through arguments