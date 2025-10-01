# Challenge 7: Exclusionary globbing
Using `[]` to exclude characters from being listed
## Solution
Navigate to `/challenge/files` and invoke `/challenge/run` with `[!pwn]*` to ignore all files that start with `p`, `w`, or `n`.
```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{gW31qmpCEFINi1Gz67h7TZXwGrg.QX2IDO0wiMwAzNzEzW}
```
## Flag
`pwn.college{gW31qmpCEFINi1Gz67h7TZXwGrg.QX2IDO0wiMwAzNzEzW}`
### Notes
- by using `!` or `^` as the first character in `[]`, the glob _inverts_ and matches characters that aren't listed, i.e. `[]` goes from a _whitelist_ to a _blacklist_