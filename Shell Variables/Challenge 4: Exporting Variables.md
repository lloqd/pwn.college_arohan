# Challenge 4: Exporting variables
Exporting variables for use across child proccesses, i.e. making them _environment_ variables
## Solution
Export the `PWN` variable, which is assigned the value `COLLEGE`, using `export`
```
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
```
Assign `PWN` to the variable `COLLEGE` with `=`
```
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```
Now, invoke `/challenge/run`
```
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{Iwr-76nMJ54GGX-WilyRSQZMlbl.QXyYTN0wiMwAzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```
## Flag
`pwn.college{Iwr-76nMJ54GGX-WilyRSQZMlbl.QXyYTN0wiMwAzNzEzW}`
### Notes
- a child process is a process that is invoked under the main _shell_
  - it does not usually inherit variables from the main _shell_ **unless** the variable is _exported_, i.e. passed to the _environment_ variables of the child process