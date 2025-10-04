# Challenge 3: Deleting newlines
Using `tr` to delete _escape sequences_ from an output
## Solution
Invoke `/challenge/run` and _pipe_ its output to `tr` to delete the _newline_ characters in the output with `-d "\n"`
```
hacker@data~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{o7FDfdJbvhnpwGlc3yfdGTgGLIJ.0VNxEzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{o7FDfdJbvhnpwGlc3yfdGTgGLIJ.0VNxEzNxwiMwAzNzEzW}`
### Notes
- to manipulate _escape sequences_ like `\n`, `\t`, etc. using tr, we need to first enclose them in `" "` to prevent the shell from interpreting the sequences itself
  - this process of enclosing characters in `" "` is known as _escaping_ them