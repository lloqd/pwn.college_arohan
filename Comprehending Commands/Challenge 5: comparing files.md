# Challenge 5: comparing files
Using the `diff` command to find differences between two given files
## Solution
Invoke `diff` with the specified files as arguments, i.e. `/challenge/decoys_only.txt` and `/challenge/decoys_and_real.txt`
```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
86a87
> pwn.college{UBKvNFAPFLtLDND_YBCev3W3IOv.01MwMDOxwiMwAzNzEzW}
```

## Flag
`pwn.college{UBKvNFAPFLtLDND_YBCev3W3IOv.01MwMDOxwiMwAzNzEzW}`

### Notes
- learnt about the `diff` command, which compares two files and outputs the difference between them