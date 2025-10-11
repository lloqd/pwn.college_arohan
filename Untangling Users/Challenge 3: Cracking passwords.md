# Challenge 3: Cracking passwords
Using _John the Ripper_ to crack the password hash of a user to log into their _shell_
## Solution
Invoke `john` on the `/challenge/shadow-leak` file provided to crack the password hash
```
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04965g/s 289.1p/s 289.1c/s 289.1C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
```
Now, we use the password obtained from _John the Ripper_ to `su` into `zardus` and invoke `/challenge/run`
```
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{YqWPK3vWoH46v5QtgWhq-q5Voi3.QX3UDN1wiMwAzNzEzW}
```
## Flag
`pwn.college{YqWPK3vWoH46v5QtgWhq-q5Voi3.QX3UDN1wiMwAzNzEzW}`
### Notes
- passwords for all users are stored in `/etc/shadow`
- when a password is inputted to `su`, it hashes it and compares it against the stored password hash in `/etc/shadow`, if they match `su` grants access to the user