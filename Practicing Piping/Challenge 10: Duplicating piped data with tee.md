# Challenge 10: Duplicating piped data with tee
Using `tee` to _duplicate_ data currently flowing through _pipes_
## Solution
Invoke `touch` to create a temporary file and intercept the `stdout` of `/challenge/pwn` that is being _piped_ through to `/challenge/college` using `tee test`
```
hacker@piping~duplicating-piped-data-with-tee:~$ touch test
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee test | /challenge/college
Processing...
WARNING: you are overwriting file test with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
```
Now, look at the contents of `test` with `cat`
```
hacker@piping~duplicating-piped-data-with-tee:~$ cat test
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "48Ajw9TV"
```
Finally, we invoke `/challenge/pwn` with the `--secret 48Ajw9TV` argument and _pipe_ its `stdout` to `/challenge/college`
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
- learnt about the `tee` command, which _duplicates_ data currently flowing through _pipes_ to any number of files provided as arguments and passes through the input it receives to the next command in the _"pipeline"_