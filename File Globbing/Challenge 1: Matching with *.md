# Challenge 1: Matching with `*`
Using the `*` glob to replace parts of a file name
## Solution
Navigate to `/challenge` with `cd c/*` to keep the argument under 4 characters (as stipulated by the challenge) and run `/challenge/run`
``` 
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{I_VZidGhpsvBNsCmeyENfALxHwn.QXxIDO0wiMwAzNzEzW} 
```
## Flag
`pwn.college{I_VZidGhpsvBNsCmeyENfALxHwn.QXxIDO0wiMwAzNzEzW}`
### Notes
- learnt about globs, which are shell expansions that let you reference files without fully typing them out or their full paths
- learnt about the `*` glob, which is expanded as a "wildcard", i.e. any part of the file name except for `/` or a leading `.`
  - the shell will replace the argument with a `*` glob with *any* files that match the pattern in the argument
  - if no files are matched, the shell leaves the glob unchanged