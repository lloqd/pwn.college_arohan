# Challenge 6: Helpful Programs
Using help arguments included in commands to read their documentation
## Solution
Invoke `/challenge/challenge` with `--help` as an argument
```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
```
Invoke the command again with the `-p` argument to get the value for `-g`
```
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 31
```
Finally, invoke `/challenge/challenge` with `-g 31`
```
hacker@man~helpful-programs:~$ /challenge/challenge -g 31
Correct usage! Your flag: pwn.college{EtrHtPTqRXsAA0vUYtPdNIe31Yt.QX3IDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{EtrHtPTqRXsAA0vUYtPdNIe31Yt.QX3IDO0wiMwAzNzEzW}`
### Notes
- some programs don't include a `man` page, but they might show instructions when invoked with a special argument
	- these are usually one of `--help`, `-h`, `-?`, etc.