# Challenge 7: Explicit relative paths, from /
Using the _relative_ path of a file/directory as part of another path
## Solution
Navigate to the `/` directory and use `./` (*relative* path to the current directory) as part of the *relative* path to `/challenge/run` to invoke the program
```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{k0E_kh0gurFPOUOpGCNHztLt0HN.QXwUTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{k0E_kh0gurFPOUOpGCNHztLt0HN.QXwUTN0wiMwAzNzEzW}`

### Notes
- learnt about `.`, which can be used in paths to refer to the _current_ directory