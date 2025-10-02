# Challenge 2: Redirecting more output
Using `>` to redirect the `stdout` of a command
## Solution
Invoke `/challenge/run` and redirect its `stdout` to `myflag`
```
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
```
The output we saw was communicated over `stderr`, to look at the command's `stdout`, wwe `cat` the `./myflag` file
```
hacker@piping~redirecting-more-output:~$ cat ./myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{g6mxXaE2mQZm2zHRUHgbsgUfw3Q.QX1YTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{g6mxXaE2mQZm2zHRUHgbsgUfw3Q.QX1YTN0wiMwAzNzEzW}`