# Challenge 2: Learning Complex Usage
Invoking commands with complex arguments 
## Solution
Invoke `/challenge/challenge` with the `--printfile` argument, which itself takes `/flag` (the path of the file to be printed)
```
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{QHU3Y0PKb6RhmkBm5aNYfT6tVsi.QX1ITO0wiMwAzNzEzW}
```
## Flag
`pwn.college{QHU3Y0PKb6RhmkBm5aNYfT6tVsi.QX1ITO0wiMwAzNzEzW}`
### Notes
- some commands have arguments that can be given arguments of their own, "nesting" arguments within each other