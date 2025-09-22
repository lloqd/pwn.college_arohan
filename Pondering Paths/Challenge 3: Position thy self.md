# Challenge 3: Position thy self
Changing the current working directory of the process and invoking a program
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