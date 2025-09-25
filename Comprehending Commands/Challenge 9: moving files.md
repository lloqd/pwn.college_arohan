# Challenge 9: moving files
Using the `mv` command to move a file to a given path
## Solution
Invoke `mv` to move `/flag` to `/tmp/hack-the-planet` using the two paths as arguments, then run `/challenge/check`
```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{0BGBIhs-RA4YuMwwBT_IX4rtw9N.0VOxEzNxwiMwAzNzEzW}
```

## Flag
`pwn.college{0BGBIhs-RA4YuMwwBT_IX4rtw9N.0VOxEzNxwiMwAzNzEzW}`
### Notes
- learnt about the `mv` command, which can move a file to a new specified path and also remove it if required
- learnt that the `mv` command has the ability to overwrite files if a duplicate file exists at the target path

### Resources
- [Geeks4Geeks - mv command](https://www.geeksforgeeks.org/linux-unix/mv-command-linux-examples/)