# Challenge 4: grepping for a needle in a haystack
Using the `grep` command to search through the contents of a file
## Solution
Invoke `grep` with `pwn.college` as the argument for the search term and `/challenge/data.txt` as the path to the search location
```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{g9k1xlnSc5AU8x5ZyxplPsrYDg1.QX3EDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{g9k1xlnSc5AU8x5ZyxplPsrYDg1.QX3EDO0wiMwAzNzEzW}`
### Notes
- learnt about the `grep` command, which can _search_ through the contents of a file
- the search term and path of the file (either _absolute_ or _relative_) are given as arguments for `grep`