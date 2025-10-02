# Challenge 5: Printing Exported Variables
Using `env` to print out vall exported variables
## Solution
Invoke `env` to print out variables and _pipe_ its `stdout` to `grep FLAG`
```
hacker@variables~printing-exported-variables:~$ env | grep FLAG
FLAG=pwn.college{86-8nHJrvhGm_LDyeF1IIWGW7cK.QX4UTN0wiMwAzNzEzW}
```
## Flag
`pwn.college{86-8nHJrvhGm_LDyeF1IIWGW7cK.QX4UTN0wiMwAzNzEzW}`
### Notes
- learnt about the `env` command, which prints out every exported variable set in the _shell_