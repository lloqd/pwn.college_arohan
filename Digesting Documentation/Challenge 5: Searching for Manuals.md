# Challenge 5: Searching For Manuals
Reading through *man*pages to find the relevant information
## Solution
After invoking `man man` as suggested by the challenge and reading through the *man*page, we see the following under `EXAMPLES` (on how to use the `man` command)
```
       man -k printf
           Search  the  short  descriptions and manual page names for the keyword printf as regular expression.  Print out any matches.  Equivalent to apropos printf.
```
This tells us that running `man -k search_term` will search through all *man*pages for any matches of the `search_term`, so we invoke `man -k flag`, and in the results we see:
```
wxhrssnlrt (1)       - print the flag!
```
Obviously, the entry for `wxhrssnlrt`  must be the entry for `/challenge/challenge`, renamed to a random string as mentioned in the challenge description, so we read its man page with `man wxhrssnlrt` and find:
```
--wxhrss NUM
              print the flag if NUM is 094
```
Finally, we invoke `/challenge/challenge` with the `--wxhrss 094` argument
```
hacker@man~searching-for-manuals:~$ /challenge/challenge --wxhrss 094
Correct usage! Your flag: pwn.college{09UUw4Ux8hUrYUTGs0U3snlrKDt.QX2EDO0wiMwAzNzEzW}
```
## Flag
`pwn.college{09UUw4Ux8hUrYUTGs0U3snlrKDt.QX2EDO0wiMwAzNzEzW}`