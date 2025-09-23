# Challenge 8: Implicit relative path
Invoke a program in the _current_ directory using its _relative_ path
## Solution
Navigate to the `/challenge` directory using `cd` and invoke the `run` file using `./run`
```
hacker@paths~implicit-relative-path:~$ cd /challenge/
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Y29MSGVyv2rBWULDDQ0pyUkBnIJ.QXxUTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{Y29MSGVyv2rBWULDDQ0pyUkBnIJ.QXxUTN0wiMwAzNzEzW}`
### Notes
- learnt that _naked_ paths do not invoke programs
	- this is because on entering a _naked_ path, the user could accidentally invoke programs stored in `~` that share names with system utilities
- so, to invoke a program present in the `cwd`, we have to point to it using `./file_name`