# Challenge 4: Matching paths with `[]`
Using `[]` to expand entire paths
## Solution
Invoke `challenge/run`  with a globbed argument that expands to the absolute paths for the files mentioned in the challenge, i.e. `/challenge/files/file_[bash]`
```
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{wqN6Ea_MoRoQZq-fHyujFGgaGeD.QX0IDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{wqN6Ea_MoRoQZq-fHyujFGgaGeD.QX0IDO0wiMwAzNzEzW}`
### Notes
- globbing happens on a path basis, i.e. entire paths can be expanded from globbed arguments