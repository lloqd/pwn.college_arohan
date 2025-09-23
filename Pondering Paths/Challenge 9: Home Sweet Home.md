# Challenge 9: Home Sweet Home
Invoke the `run` program which writes a copy of the flag to a file that the user specifies as an argument, as long as said argument follows the constraints given below:
1. Your argument must be an _absolute_ path. <br>
2. The path must be inside your `home` directory. <br>
3. Before expansion, your argument must be **three characters or less**.

## Ssolution
Based on the constraints for the argument, we can use `~` to represent the `home` directory, and use a file name that's one character long to satisfy the **three characters or less** requirement, hence the path is `~/f`
```
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{INjGi0C2DyB-sxWmK6yRr6cvq1q.QXzMDO0wiMwAzNzEzW}
```

### Flag
`pwn.college{INjGi0C2DyB-sxWmK6yRr6cvq1q.QXzMDO0wiMwAzNzEzW}`
### Notes
- learnt about using `~` to represent the `home` directory
- learnt that it's expansion is an _absolute_ path, and in a path containing multiple `~` , only the leading `~` is considered for expansion
- when running `cd` without an argument, it uses the `home` directory as its default destination
