# Challenge 3: Finding Sessions

## Solution

```
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
	139.pts-0.terminal-multiplexing~detaching-and-attaching	(Remote or dead)
	144.session_410f181ef98f799a	(Detached)
	147.session_5e9de5810a84c7d0	(Detached)
	150.session_6618e4dbda25513f	(Detached)
4 Sockets in /home/hacker/.screen.
```
`hacker@terminal-multiplexing~finding-sessions:~$ screen -r 147`
```
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{IH81fk9-lxJT7Mg6pLJMLw2MXj5.01N4IDOxwiMwAzNzEzW}
pwn.college{IH81fk9-lxJT7Mg6pLJMLw2MXj5.01N4IDOxwiMwAzNzEzW}
```
## Flag
`pwn.college{IH81fk9-lxJT7Mg6pLJMLw2MXj5.01N4IDOxwiMwAzNzEzW}`
### Notes
-