# Challenge 8: Reading Files
Using `read` to assign a variable with a file
## Solution
Invoke `read PWN` with the `<` operator, reading the value of `/challenge/read_me` into the `PWN` variable
```
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{sIQp2nZFojBQhHJJems4zGO62Ln.QXwIDO0wiMwAzNzEzW}
```
## Flag
`pwn.college{sIQp2nZFojBQhHJJems4zGO62Ln.QXwIDO0wiMwAzNzEzW}`