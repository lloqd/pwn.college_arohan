# Challenge 11: Scripting with Multiple Conditions

## Solution

```
#!/bin/bash
if [ "$1" = "hack" ]
then
    echo "the planet"
elif [ "$1" = "pwn" ]
then
    echo "college"
elif [ "$1" = "learn" ]
then
    echo "linux"
else
    echo "unknown"
fi
```

```
hacker@chaining~scripting-with-multiple-conditions:~$ vim /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{cj7K9BBHuIbFbnkqhS7tDz6uRrW.0FOzMDOxwiMwAzNzEzW}
```
## Flag
`pwn.college{cj7K9BBHuIbFbnkqhS7tDz6uRrW.0FOzMDOxwiMwAzNzEzW}`
### Notes
-