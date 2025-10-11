# Challenge 5: Detaching and Attaching (tmux)

## Solution

```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
```

```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
```

```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux a
```

```
Congratulations, here is your flag: pwn.college{YdadDEtM-16TDQBLBrc7N7FpqK0.0VO4IDOxwiMwAzNzEzW}
```
## Flag
`pwn.college{YdadDEtM-16TDQBLBrc7N7FpqK0.0VO4IDOxwiMwAzNzEzW}`
### Notes
-