# Challenge 8: The SUID Bit

## Solution

```
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{cic5xpWQLiRI-cn627JaImOqmxJ.QXzEjN0wiMwAzNzEzW}
```
## Flag
`pwn.college{cic5xpWQLiRI-cn627JaImOqmxJ.QXzEjN0wiMwAzNzEzW}`
### Notes
-