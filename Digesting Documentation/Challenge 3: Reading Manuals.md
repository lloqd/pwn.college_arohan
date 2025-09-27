# Challenge 3: Reading Manuals
Using the `man` command to read the included documentation for commands
## Solution
Invoke `man` with `challenge` as an argument
```
hacker@man~reading-manuals:~$ man challenge
```
Reading through the `man` page, we see this argument mentioned under `DESCRIPTION`
```
-cpftue NUM
              print the flag if NUM is 118
```
So, we invoke `/challenge/challenge` with the aforementioned argument
```
hacker@man~reading-manuals:~$ /challenge/challenge --cpftue 118
Correct usage! Your flag: pwn.college{IAcNPpf1XIZ1Htu89PAeAH8lVUv.QX0EDO0wiMwAzNzEzW}
```
## Flag
`pwn.college{IAcNPpf1XIZ1Htu89PAeAH8lVUv.QX0EDO0wiMwAzNzEzW}`
### Notes
- learnt about the `man` command, which displays a manual page for the command passed as an argument
- *man*pages are stored at `/usr/share/man`, but we can better query them using man
    - the *man*page can be navigated using the arrow keys and the `PgUp/PgDn` keys