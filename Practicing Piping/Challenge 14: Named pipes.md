# Challenge 14: Named pipes
Using a _persistent_ named pipe (_FIFO_)  instead of a temporary pipe, like the ones created by `|`
## Solution
Invoke `mkfifo` to create a _FIFO_ at the given path and redirect the `stdout` of `/challenge/run` to it
```
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
```
Since the terminal will be blocked till both the read and write side of the _FIFO_ are clear, we open a new terminal and invoke `cat` to open the read side
```
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{05WbqWFiEhA8PBf4jltSj6_qsLy.01MzMDOxwiMwAzNzEzW}
```
## Flag
`pwn.college{05WbqWFiEhA8PBf4jltSj6_qsLy.01MzMDOxwiMwAzNzEzW}`
### Notes
- learnt about _FIFOs_, (First (byte) In, First (byte) Out), which are _persistent_ named pipes, some of the advantages of which are:
  - their path can be controlled
  - any process can write to them by path
  - they are listed with `ls` and treated as files
  - they don't save anything to disk, everything through a _FIFO_ passes directly between processes in memory
  - data from a _FIFO_ isn't stored unlike with files
  - multiple processes can read/write to and from a _FIFO_