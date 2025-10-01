# Challenge 5: Multiple globs
Using multiple globs in a single argument
## Solution
Navigate to `/challenge/files` and invoke `/challenge/run` with `*p*`, which expands to every word that contains the letter `p` while keeping the argument only 3 characters long
```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{EVOc0TxkWwanhQXb2e749tgF7L4.0lM3kjNxwiMwAzNzEzW}
```

## Flag
`pwn.college{EVOc0TxkWwanhQXb2e749tgF7L4.0lM3kjNxwiMwAzNzEzW}`
### Notes
- multiple globs can be expanded at one time in a single argument
  - eg: `/h?m?` expands to `/home`