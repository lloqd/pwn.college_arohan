# Challenge 3: Position thy self
Changing the _current working directory_ of the shell and invoking a program from a specified directory
## Solution
Navigate to the `/var` directory as instructed by the program and then invoke `run` using `/challenge/run`
```
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /var directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /var/
hacker@paths~position-thy-self:/var$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{YIxAuriRu3ZJPuON44cRGMB2z3w.QX2QTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{YIxAuriRu3ZJPuON44cRGMB2z3w.QX2QTN0wiMwAzNzEzW}`

### Notes
- learnt about `cd` or the **c**hange **d**irectory command, which changes the **c**urrent **w**orking **d**irectory (`cwd`) of the process (usually the shell)
- learnt about `~`, which represents the current path of the shell