# Challenge 4: Extracting the first few lines with head
Using `head` to only display the first few lines of an output
## Solution
Invoke `/challenge/pwn`, _pipe_ its output to `head` and display the first _7_ lines (as mentioned in the challenge description) and finally _pipe_ it to `/challenge/college`
```
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{YgxScqqhw7vMer0VsbB2UOR-ogi.0lNxEzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{YgxScqqhw7vMer0VsbB2UOR-ogi.0lNxEzNxwiMwAzNzEzW}`
### Notes
- learnt about the `head` command, which is used to display the first few lines of its input, defaults to _10_ but can be configured with the `-n` argument