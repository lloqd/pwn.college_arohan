# Challenge 6: Grepping stored results
Redirecting the `stdout` of a program to a file and searching through it using `grep`
## Solution
Invoke `/challenge/run` and redirect its `stdout` to `/tmp/data.txt` with the `>` operator
```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
```
Now, invoke `grep` to search for the flag in `/tmp/data.txt`
```
hacker@piping~grepping-stored-results:~$ grep pwn.college /tmp/data.txt
pwn.college{AX6QPYcI8iAjWoZXgw8IFqR3yV0.QX4EDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{AX6QPYcI8iAjWoZXgw8IFqR3yV0.QX4EDO0wiMwAzNzEzW}`