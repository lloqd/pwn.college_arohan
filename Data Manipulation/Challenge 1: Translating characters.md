# Challenge 1: Translating characters
Using `tr` to _translate_ characters
## Solution
Invoke `/challenge/run` and _pipe_ its output to `tr` to change the case of all characters
```
hacker@data~translating-characters:~$ /challenge/run | tr QWERTYUIOPASDFGHJKLZXCVBNMqwertyuiopasdfghjklzxcvbnm qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM
yOUR CASE-SWAPPED FLAG:
pwn.college{8kUEQwqIgd-BW1qNaIEH2eZg_ul.01MxEzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{8kUEQwqIgd-BW1qNaIEH2eZg_ul.01MxEzNxwiMwAzNzEzW}`
### Notes
- learnt about the `tr` command, which translates the characters it receives from `stdin` and prints them to `stdout`
  - it translates the characters provided in the first argument to the characters provided in the second argument