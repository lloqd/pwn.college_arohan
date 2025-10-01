# Challenge 2: Matching with `?`
Using the `?` glob to match one character in a file name
## Solution
Navigate to `/challenge` with `cd /?ha??enge` to avoid using `c` or `l` in the argument (as mentioned in the challenge) and run `/challenge/run`
```
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{oHsuitOsU8M57oiY0eUX1tScN7e.QXyIDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{oHsuitOsU8M57oiY0eUX1tScN7e.QXyIDO0wiMwAzNzEzW}`
### Notes
- learnt about the `?` glob, which is expanded as a "wildcard", similar to `*`, but only for single characters