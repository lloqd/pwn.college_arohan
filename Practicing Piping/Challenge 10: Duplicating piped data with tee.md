# Challenge 10: Duplicating piped data with tee

## Solution

```
hacker@piping~duplicating-piped-data-with-tee:~$ touch test
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee test | /challenge/college
Processing...
WARNING: you are overwriting file test with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
```

```
hacker@piping~duplicating-piped-data-with-tee:~$ cat test
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "48Ajw9TV"
```

```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 48Ajw9TV | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{48Ajw9TVMBQul0I1yZuKDgY7yHz.QXxITO0wiMwAzNzEzW}
```
## Flag
`pwn.college{48Ajw9TVMBQul0I1yZuKDgY7yHz.QXxITO0wiMwAzNzEzW}`
### Notes
-