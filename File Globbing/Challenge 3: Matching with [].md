# Challenge 3: Matching with `[]`
Using `[]` to match one character out of the ones mentioned in the brackets
## Solution
Navigate to `/challenge/files`, then run `/challenge/run` with `file_[bash]` as the argument to have the glob expand into the files mentioned in the challenge
```
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{MFsDlqJkB5CBTxP8AqWH15vuTS1.QXzIDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{MFsDlqJkB5CBTxP8AqWH15vuTS1.QXzIDO0wiMwAzNzEzW}`
### Notes
- learnt about `[]`, which acts a single character wildcard (like `?`), but only for a set of characters, those which are specified between the brackets