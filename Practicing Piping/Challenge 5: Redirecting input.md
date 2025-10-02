# Challenge 5: Redirecting input
Using `<` to redirect files to the `stdin` of programs 
## Solution
Invoke `echo COLLEGE` and redirect its `stdout` to `PWN` with `>`
```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
```
Now, invoke `/challenge/run` and redirect `PWN` to its `stdin` with `<`
```
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{AiIGUCur_Ec0kxVID7kezCHV20q.QXwcTN0wiMwAzNzEzW}
```
## Flag
`pwn.college{AiIGUCur_Ec0kxVID7kezCHV20q.QXwcTN0wiMwAzNzEzW}`
### Notes
- learnt about the `<` operator, which can be used to redirect files to the `stdin` stream  of a program