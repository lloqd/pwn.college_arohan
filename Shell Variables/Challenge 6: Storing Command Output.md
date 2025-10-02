# Challenge 6: Storing Command Output
Using _command substitution_ to store the output of a command to a variable
## Solution
Assign `PWN` with the output of `/challenge/run` by enclosing it in `()` and prepending it with a `$`
```
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{0JnsFRx-JM4rd8CfcJoyxtwcB-G.QX1cDN1wiMwAzNzEzW}
```
## Flag
`pwn.college{0JnsFRx-JM4rd8CfcJoyxtwcB-G.QX1cDN1wiMwAzNzEzW}`
### Notes
- learnt about _command substitution_, i.e. replacing a command with its output using `$(/path)`, which can be assigned to variables and such