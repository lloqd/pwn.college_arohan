# Challenge 13: Split-piping stderr and stdout
Piping from two streams in one command to separate paths
## Solution
Invoke `/challenge/hack`, which will give an output to its `stdout` and its `stderr` <br>
To pipe `stderr` to `/challenge/the`, we use its _FD_ number (`2`) and redirect it to the process substituted path `(/challenge/the)`<br>
To pipe `stdout` to `/challenge/file`, we simply use the `|` operator with its path
```
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{YyxwgDIjwlf77DUkix3EiQn9hY6.QXxQDM2wiMwAzNzEzW}
```
## Flag
`pwn.college{YyxwgDIjwlf77DUkix3EiQn9hY6.QXxQDM2wiMwAzNzEzW}`