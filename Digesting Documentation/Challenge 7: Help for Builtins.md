# Challenge 7: Help for Builtins
Using the _shell_ builtin `help` to get documentation for other _shell_ builtins
## Solution
Invoke `help` with `challenge` as an argument
```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune		display a fortune
      --version		display the version
      --secret VALUE	prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "wZceP74k".
```
Now, invoke `challenge` with the `--secret` argument
```
hacker@man~help-for-builtins:~$ challenge --secret wZceP74k
Correct! Here is your flag!
pwn.college{wZceP74kDdLc3V03G1zNVr-LFyX.QX0ETO0wiMwAzNzEzW}
```

## Flag
`pwn.college{wZceP74kDdLc3V03G1zNVr-LFyX.QX0ETO0wiMwAzNzEzW}`
### Notes
- learnt about `builtins`, which are commands built into the shell itself rather than being separate programs
- the `help` builtin can list all the shell builtins when invoked without an argument
	- `help` can also display info about another builtin -  by passing it as an argument