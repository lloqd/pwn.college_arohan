# Challenge 5: Position yet elsewhere
Changing the current working directory of the process and invoking a program
## Solution
Navigate to the `/home` directory as instructed by the program and then invoke `run` using `/challenge/run`
```
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /home directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /home
hacker@paths~position-yet-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{k0cBUUOitXckeo3b_z3ffcxwaa9.QX4QTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{k0cBUUOitXckeo3b_z3ffcxwaa9.QX4QTN0wiMwAzNzEzW}`
