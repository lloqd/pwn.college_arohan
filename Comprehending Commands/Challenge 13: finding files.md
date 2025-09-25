# Challenge 13: finding files
Using the `find` command to search for a file
## Solution
Invoke `find` at `/` with the search term being `flag`, given as an argument with `-name flag`, and on identifying the correct `flag` file, read its contents with `cat`
```
hacker@commands~finding-files:~$ find / -name flag
find: ‘/tmp/tmp.TpSOPGOVKK’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
/usr/lib/python3/dist-packages/jedi/third_party/typeshed/stdlib/3/email/mime/flag
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
find: ‘/var/cache/apt/archives/partial’: Permission denied
find: ‘/var/cache/ldconfig’: Permission denied
find: ‘/var/cache/private’: Permission denied
find: ‘/var/lib/apt/lists/partial’: Permission denied
find: ‘/var/lib/mysql-files’: Permission denied
find: ‘/var/lib/private’: Permission denied
find: ‘/var/lib/mysql’: Permission denied
find: ‘/var/lib/mysql-keyring’: Permission denied
find: ‘/var/lib/php/sessions’: Permission denied
find: ‘/var/log/private’: Permission denied
find: ‘/var/log/apache2’: Permission denied
find: ‘/var/log/mysql’: Permission denied
find: ‘/run/mysqld’: Permission denied
find: ‘/run/sudo’: Permission denied
find: ‘/root’: Permission denied
/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
hacker@commands~finding-files:~$ cat /usr/lib/python3/dist-packages/jedi/third_party/typeshed/stdlib/3/email/mime/flag
pwn.college{Iml6M9vBQAuGUyrDeSSxN2YoV6p.QXyMDO0wiMwAzNzEzW}
```

## Flag
`pwn.college{Iml6M9vBQAuGUyrDeSSxN2YoV6p.QXyMDO0wiMwAzNzEzW}`
### Notes
- learnt about the `find` command, which can be used to find files (`¯\_(ツ)_/¯`)
- when provided with (optional) arguments, `find`'s search criteria and search location can be defined
	- these default to the `cwd` and "no" criteria, wherein `find` will list every file in the search directory
- `find` searches _recursively_, i.e. through all of the sub-directories of the search directories and through all of their sub-directories and so on 