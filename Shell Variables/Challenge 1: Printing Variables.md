# Challenge 1: Printing Variables
Printing out variables using `echo $VAR_NAME`
## Solution
Invoke `echo` with the `$` prefix before the variable name to print out the `FLAG` variable
```
hacker@variables~printing-variables:~$ echo $FLAG
pwn.college{I85XMvtpzLPB9aW__lkzl9M4Tko.QX3UTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{I85XMvtpzLPB9aW__lkzl9M4Tko.QX3UTN0wiMwAzNzEzW}`
### Notes
- `echo` can be used to print out _shell variables_ by using `$VAR_NAME` as an argument for `echo`