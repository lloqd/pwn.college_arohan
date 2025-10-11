# Challenge 1: Becoming root with su
Using the `su` command to gain _root_ privileges
## Solution
Invoke `su` and input the _root_ password given in the challenge's description to elevate to _root_ then invoke `cat`
```
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{gc00O3hdJz3qxRbaS9AZTEpUqNI.QX1UDN1wiMwAzNzEzW}
```
## Flag
`pwn.college{gc00O3hdJz3qxRbaS9AZTEpUqNI.QX1UDN1wiMwAzNzEzW}`
### Notes
- learnt about the `su` (substitute user) command, which has the `SUID` bit set, therefore it runs as *root* and can hence start a *root* shell
- before allowing the user to elevate to _root_, `su` asks for the _root_ password, which is rarely available on modern systems and is the reason for `su` becoming obsolete