# Challenge 7: Reading Input
Using `read` to read data from `stdin` and assign it to a variable
## Solution
Invoke `read` (with `-p` to display a prompt) to assign `stdin` to the `PWN` variable
```
hacker@variables~reading-input:~$ read -p "INPUT:" PWN
INPUT:COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{I4gXgYnDEtrnV2WVpcr1DrfnB0_.QX4cTN0wiMwAzNzEzW}
```
## Flag
`pwn.college{I4gXgYnDEtrnV2WVpcr1DrfnB0_.QX4cTN0wiMwAzNzEzW}`
### Notes
- learnt about the `read` builtin, which can be used to assign `stdin` to a variable