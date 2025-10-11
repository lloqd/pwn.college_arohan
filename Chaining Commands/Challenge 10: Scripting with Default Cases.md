# Challenge 10: Scripting with Default Cases

## Solution

```
#!/bin/bash
if [ "$1" == "pwn" ]
then
    echo "college"
else
    echo "nope"
fi
```

```
hacker@chaining~scripting-with-default-cases:~$ vim /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{kk5eeuQPXKq9kba6gqKz7jFnLAr.01NzMDOxwiMwAzNzEzW}
```
## Flag
`pwn.college{kk5eeuQPXKq9kba6gqKz7jFnLAr.01NzMDOxwiMwAzNzEzW}`
### Notes
-