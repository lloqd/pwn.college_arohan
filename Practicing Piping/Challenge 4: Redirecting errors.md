# Challenge 4: Redirecting errors
Using _file descriptors_ with `>` to redirect specific output streams to given files
## Solution
Invoke `/challenge/run` and redirect its `stdout` to `myflag` with `1>` and its `stderr` to `instructions` with `2>`
```
hacker@piping~redirecting-errors:~$ /challenge/run 1> myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{IxydhsxQrK7kWdlcKUM2DqFoofz.QX3YTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{IxydhsxQrK7kWdlcKUM2DqFoofz.QX3YTN0wiMwAzNzEzW}`
### Notes
- learnt about _file descriptors_, which are numbers assigned to the default I/O streams that can be used to reference them from the _shell_
  - `stdin`: 0
  - `stdout`: 1
  - `stderr`: 2
- we can prefix the `>` operator with a _FD_ to specify which I/O stream is to be redirected
  - when a _FD_ is not mentioned in a command, it is implicitly taken to be `1`