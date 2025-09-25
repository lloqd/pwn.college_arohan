# Challenge 11: An Epic Filesystem Quest
Using the commands learnt previously in a ~~wild goose chase~~ treasure hunt of sorts
## Solution
We start by listing all contents of `/` using `ls /`
```
hacker@commands~an-epic-filesystem-quest:~$ ls /
LEAD  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
```
On observing, the `/LEAD` file looks it could hold the clue, so we read its contents using `cat /LEAD`
```
hacker@commands~an-epic-filesystem-quest:~$ cat /LEAD
Tubular find!
The next clue is in: /usr/share/doc/arping

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
```
Using the hint, we list the contents of `/usr/share/doc/arping` using `ls`
```
hacker@commands~an-epic-filesystem-quest:~$ ls /usr/share/doc/arping
ALERT-TRAPPED  README.Debian  README.gz  changelog.Debian.gz  copyright  examples
```
Similar to `/LEAD`, we read `./ALERT-TRAPPED`'s contents with `cat`
```
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/share/doc/arping/ALERT-TRAPPED
Yahaha, you found me!
The next clue is in: /opt/pwndbg/.venv/lib/python3.8/site-packages/mako-1.3.10.dist-info
```
Similarly to what we've done before, we keep repeating this cycle, eventually reaching here:
```
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/fonts/Neo-Euler/Symbols/Regular/DISPATCH
Tubular find!
The next clue is in: /usr/local/lib/python3.8/dist-packages/jupyterlab_server/templates

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
```
Unlike the previous cases, this time we need to `cd` into the directory to read the clue, where we will run `ls` to get the directory's contents
```
hacker@commands~an-epic-filesystem-quest:~$ cd /usr/local/lib/python3.8/dist-packages/jupyterlab_server/templates
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyterlab_server/templates$ ls
403.html  DOSSIER  error.html  index.html
```
Again, invoke `cat` to read through `./DOSSIER`
```
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyterlab_server/templates$ cat ./DOSSIER
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/misc/altera-stapl
```
Like so, we keep moving through the clues to eventually reach the flag at `/usr/share/doc/python3-ptyprocess/README`
```
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyterlab_server/templates$ cat /usr/share/doc/python3-ptyprocess/README
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{U1WAWPwUmGsersNXTFSjMn5VFy5.QX5IDO0wiMwAzNzEzW}
```
### Flag
`pwn.college{U1WAWPwUmGsersNXTFSjMn5VFy5.QX5IDO0wiMwAzNzEzW}`
