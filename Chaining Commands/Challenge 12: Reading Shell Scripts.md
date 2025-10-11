# Challenge 12: Reading Shell Scripts

## Solution

```
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
	echo "CORRECT! Your flag:"
	cat /flag
else
	echo "Read the /challenge/run file to figure out the correct password!"
fi
```

```
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{AgbQFpb4SbRXyOe2xz4RceDVSsL.0lMwgDOxwiMwAzNzEzW}
```

## Flag
`pwn.college{AgbQFpb4SbRXyOe2xz4RceDVSsL.0lMwgDOxwiMwAzNzEzW}`
### Notes
-