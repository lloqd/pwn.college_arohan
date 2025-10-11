# Challenge 2: Other users with su
Using the `su` command to switch to a specified user
## Solution
Invoke `su zardus` to switch to `zardus`'s shell, then invoke `cat`
```
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{kIBqz5RW7da4s8h7cIb4417WzF-.QX2UDN1wiMwAzNzEzW}
```
## Flag
`pwn.college{kIBqz5RW7da4s8h7cIb4417WzF-.QX2UDN1wiMwAzNzEzW}`
### Notes
- `su` can also be used to switch to a given user's shell by giving their username as an argument and providing their password when prompted