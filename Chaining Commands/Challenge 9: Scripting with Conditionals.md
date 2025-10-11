# Challenge 9: Scripting with Conditionals

## Solution

```
#!/bin/bash
if ["$1" = "pwn"]
then
    echo "college"
fi
```

```
hacker@chaining~scripting-with-conditionals:~$ nano /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{swQ2BjNvspSlV-EvWRRBmbQXP6A.0lNzMDOxwiMwAzNzEzW}
```
## Flag
`pwn.college{swQ2BjNvspSlV-EvWRRBmbQXP6A.0lNzMDOxwiMwAzNzEzW}`
### Notes
-