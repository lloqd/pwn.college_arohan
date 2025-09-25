# Challenge 1: cat, not the pet, but the command!
Using the `cat` command to read out the contents of a file
## Solution
Invoke the `cat` command and provide the path `./flag` as an argument 
```
hacker@commands~cat-not-the-pet-but-the-command:~$ cat ./flag
pwn.college{Ei2Uxi__c0jG0oQubahetl8hznX.QXxcTN0wiMwAzNzEzW}
```

## Flag
`pwn.college{Ei2Uxi__c0jG0oQubahetl8hznX.QXxcTN0wiMwAzNzEzW}`

### Notes
- learnt about the `cat` command, which can be used to read out the contents of a file
- when multiple files are provided as arguments, `cat` will con*cat*enate their contents into one output
- if no arguments are given, `cat` directly outputs the terminal input