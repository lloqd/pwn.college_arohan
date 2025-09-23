# Challenge 6: Implicit relative paths, from /
Using the _relative_ path of a file to invoke the program
## Solution
Navigate to `/` and use the _relative_ path of `/challenge/run` i.e. `challenge/run` to invoke the program
```
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wxUE_171utuCiIljCARN1G6sHnX.QX5QTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{wxUE_171utuCiIljCARN1G6sHnX.QX5QTN0wiMwAzNzEzW}`

### Notes
- learnt about the _relative_ path, a path that is interpreted relative to the `cwd`
- learnt about `..`, which represents the _parent_ directory (the directory present one level above the `cwd`)