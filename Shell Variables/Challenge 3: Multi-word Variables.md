# Challenge 3: Multi-word Variables
Assigning a string that includes spaces to a variable using `" "`
## Solution
Assign `PWN` with the value `COLLEGE YEAH` by enclosing the string in `" "`
```
hacker@variables~multi-word-variables:~$ PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{ol5qNqztCsbxuCg2HNwdrBEke-W.QXwYTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{ol5qNqztCsbxuCg2HNwdrBEke-W.QXwYTN0wiMwAzNzEzW}`
### Notes
- by using `" "`, the _shell_ interprets the content between the quotes as a single token and assigns it to the variable