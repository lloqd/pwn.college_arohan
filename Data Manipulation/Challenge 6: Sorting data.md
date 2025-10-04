# Challenge 6: Sorting data
Using `sort` to _sort_ text
## Solution
Invoke `sort` on `/challenge/flags.txt` with `-r` to sort the file in reverse alphabetical order and grab the first flag (as mentioned in the challenge description)
```
hacker@data~sorting-data:~$ sort /challenge/flags.txt -r
pwn.college{kcwFFTppmHiWB3ymmQFZvuTTqyp.0FM0MDOxwiMwAzNzEzW}
...
```
## Flag
`pwn.college{kcwFFTppmHiWB3ymmQFZvuTTqyp.0FM0MDOxwiMwAzNzEzW}`
### Notes
- learnt about the `sort` command, which organizes its input alphabetically (by default)
- `sort` has multiple parameters for sorting that the user can select, being:
  - `-r`: reverse alphabetical
  - `-n`: numeric sort
  - `-u`: unique only
  - `-R`: random order