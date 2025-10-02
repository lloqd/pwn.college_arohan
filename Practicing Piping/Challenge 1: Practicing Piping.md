# Challenge 1: Redirecting output
Using `>` to redirect the `stdout` of a command
## Solution
Invoke `echo PWN` and redirect its `stdout` to `COLLEGE` with `>`
```
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your
flag:
pwn.college{UbYyT8Jq0VhPiRc7dwpE3V7bea5.QX0YTN0wiMwAzNzEzW}
```
## Flag
`pwn.college{UbYyT8Jq0VhPiRc7dwpE3V7bea5.QX0YTN0wiMwAzNzEzW`
### Resources
- [Unix Shell: The Art of I/O Redirection - Benjamin Cane](https://web.archive.org/web/20220629044814/http://bencane.com:80/2012/04/16/unix-shell-the-art-of-io-redirection/) (for the entire module)
### Notes
- learnt about the default I/O streams in Linux, which are used to interact with user input and program outputs:
  - `stdin` (Standard Input): through which input is taken - usually through the user's keyboard for the terminal
  - `stdout` (Standard Output): through which non-error output is given - usually to the terminal display for _shell_ commands
  - `stderr` (Standard Error): through which error output is given - usually to the terminal as well
- learnt about the `>` redirection operator, which redirects the `stdout` of the process on the left to the `stdin` of the file on the right and overwrites its contents