# Challenge 9: Multiple options for tab completion
Using the `Tab` key to auto complete and navigating through multiple options
## Solution
Try to invoke `cat` and type out `/challenge/files/p` as an argument and press the `Tab` key, the shell will auto complete to `/challenge/files/pwn`, and on pressing `Tab` again, the options listed below will be printed
```
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter
pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking
```
Now, invoke `cat` with `/challenge/files/pwncollege-flag`
```
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{ceX-Dtk-iiX03HXr3CXaT6RUnls.0lN0EzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{ceX-Dtk-iiX03HXr3CXaT6RUnls.0lN0EzNxwiMwAzNzEzW}`
### Notes
- when _tab completion_ is executed, `bash` will expand until the first point where there exist multiple options, and on pressing `Tab` a second time, it will print out these options