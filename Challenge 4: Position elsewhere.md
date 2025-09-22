# Challenge 4: Position elsewhere
Changing the current working directory of the process and invoking a program
## Solution
Navigate to the `/sys/kernel` directory as instructed by the program and then invoke `run` using `/challenge/run`
```
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /sys/kernel directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /sys/kernel
hacker@paths~position-elsewhere:/sys/kernel$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{YVLfgnPQDlvo_9ZsN3qrlSI8gbl.QX3QTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{YVLfgnPQDlvo_9ZsN3qrlSI8gbl.QX3QTN0wiMwAzNzEzW}`