# Challenge 2:  Deleting characters
Delete characters from text using `tr -d`
## Solution
Invoke `/challenge/run` and _pipe_ through the output to `tr` to delete `^%`
```
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{4zQOyCCLRUelvWU398H_6jlZwnS.0FNxEzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{4zQOyCCLRUelvWU398H_6jlZwnS.0FNxEzNxwiMwAzNzEzW}`
### Notes
- `tr` can also delete characters by specifying the `-d` flag and mentioning the characters to delete in the next field