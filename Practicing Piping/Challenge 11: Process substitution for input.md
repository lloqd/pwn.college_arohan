# Challenge 11: Process substitution for input
Using _process substitution_ to use programs in place of files as arguments for another command
## Solution
Invoke `diff` on `/challenge/print_decoys` and `/challenge/print_decoys_and_flag` which are _process substituted_ with `<(/path)`
```
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
2a3
> pwn.college{k0CY1z0Grws14K-kownw6HBhFY2.0lNwMDOxwiMwAzNzEzW}
```

## Flag
`pwn.college{k0CY1z0Grws14K-kownw6HBhFY2.0lNwMDOxwiMwAzNzEzW}`
### Notes
- learnt about _process substitution_, i.e. hooking up the inputs/outputs of programs to the _arguments_ of other commands
  - eg: to _read_ from a program, use <(program), which runs it and sends its output to a temporary file that the _shell_ uses for the `stdin` of the first command
- `bash` replaces the _process substituted_ programs before the shell command is even run, so it never even sees them, only the temporary file that the _shell_ creates!