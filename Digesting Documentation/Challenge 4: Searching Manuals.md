# Challenge 4: Searching Manuals
Searching through *man*pages using `vi` commands
## Solution
Invoke `man` for the `challenge` command
```
hacker@man~searching-manuals:~$ man challenge
```
Search the *man*page using `/flag` and going through the results with the `n` key, we see
```
		--ug   This argument will give you the flag!
```
So, we invoke `/challenge/challenge` with the `--ug` argument
```
hacker@man~searching-manuals:~$ /challenge/challenge --ug
Initializing...
Correct usage! Your flag: pwn.college{oquSHmM8XwzXXeY66hjD-luzp2m.QX1EDO0wiMwAzNzEzW}
```
## Flag
`pwn.college{oquSHmM8XwzXXeY66hjD-luzp2m.QX1EDO0wiMwAzNzEzW}`
### Notes
- to search through a `man` page (essentially a text file opened in `vi`), we can use `/` to search forwards from the current position, or `?` to search backwards
- to go through the search results, we can use `n` & `N` to navigate forwards/backwards between them