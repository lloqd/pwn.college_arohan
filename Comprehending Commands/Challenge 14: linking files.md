# Challenge 14: linking files
Using the `ln` command to create _symbolic_ links
## Solution
Invoke `ln` with the `-s` argument to create _symbolic_ links, linking `/home/hacker/not-the-flag` to `/flag` , i.e. whenever the former is accessed, Linux will redirect the process to access `/flag` instead
```
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{IMyb20NTj92Lk58imgKxpvvWJCc.QX5ETN1wiMwAzNzEzW}
```

## Flag
`pwn.college{IMyb20NTj92Lk58imgKxpvvWJCc.QX5ETN1wiMwAzNzEzW}`
### Notes
- learnt about links, _hard_ and _soft_ (_symbolic_)
	- a _hard_ link creates another directory entry for the same file
	- a _soft_ link redirects processes to access the linked file/directory whenever they want to access the link
- when a _symlink_ (_symbolic_ link) is modified, the original file is not affected, whereas with a _hard_ link, both the link and the original are modiifed.

### References
- [reddit: r/linux4noobs](https://reddit.com/r/linux4noobs)