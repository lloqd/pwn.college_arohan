# Challenge 3: Finding Commands
Using `which` to find the _absolute path_ of a command
## Solution
Invoke `which` to find the path of `win` and invoke `cat` on `flag` present in the same directory (as mentioned in the challenge's description)
```
hacker@path~finding-commands:~$ which win
/challenge/paths/11140/win
hacker@path~finding-commands:~$ cat /challenge/paths/11140/flag
pwn.college{8DDthEEzRGzAQLsx2uFPzsccTUW.01NzEzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{8DDthEEzRGzAQLsx2uFPzsccTUW.01NzEzNxwiMwAzNzEzW}`
### Notes
- learnt about the `which` command, which looks through `PATH` to find the first file that matches with the argument passed - just like what the _shell_ does when a command is invoked