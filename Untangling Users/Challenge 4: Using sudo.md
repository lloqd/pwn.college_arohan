# Challenge 4: Using sudo
Using `sudo` to run a command with elevated privileges
## Solution
Prepend `cat /flag` with `sudo` to run the command with elevated privileges
```
hacker@users~using-sudo:~$ sudo cat /flag
pwn.college{g4IAaZOfxDXLsV0Tr2HjPX2UVmo.QX4UDN1wiMwAzNzEzW}
```
## Flag
`pwn.college{g4IAaZOfxDXLsV0Tr2HjPX2UVmo.QX4UDN1wiMwAzNzEzW}`
### Notes
- learnt about `sudo` (superuser do), which defaults to running a command as `root` instead of launching a `root` shell like `su` does
- instead of asking for the `root` password, `sudo` checks policies defined in `/etc/sudoers` to determine whether the user is authorized to run commands as `root` or not