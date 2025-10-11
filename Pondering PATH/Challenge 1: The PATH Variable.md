# Challenge 1: The PATH Variable
Modifying the value of `PATH`
## Solution
Modify the `PATH` variable to be empty and invoke `/challenge/run`
```
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{sgedHyV0UKjxKgM7rhwHQzvdnlA.QX2cDM1wiMwAzNzEzW}
```
## Flag
`pwn.college{sgedHyV0UKjxKgM7rhwHQzvdnlA.QX2cDM1wiMwAzNzEzW}`
### Notes
- the `PATH` variable stores directory paths of commands 
- the _shell_ searches through `PATH` to run said commands when they are invoked by the user