# Challenge 12: Writing to multiple programs
Using `tee` to duplicate to two commands using _process substitution_
## Solution
Invoke `/challenge/hack`, _pipe_ its `stdout` with `|` to `tee`, which duplicates the data to a _process substituted_ `/challenge/the` and then passes it forward to the `stdin` of `/challenge/planet`
```
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) | /challenge/planet
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{cbgSQ9g6SVf1cMEryz6L1NXmfl8.QXwgDN1wiMwAzNzEzW}
```

## Flag
`pwn.college{cbgSQ9g6SVf1cMEryz6L1NXmfl8.QXwgDN1wiMwAzNzEzW}`