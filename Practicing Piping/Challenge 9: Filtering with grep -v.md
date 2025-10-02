# Challenge 9: Filtering with grep -v
_Inverting_ `grep`'s filters with `-v` and filtering through the output of a program with `|`
## Solution
Invoke `/challenge/run`, _pipe_ its `stdout` to `grep` and invert it using `-v` to exclude lines containing `DECOY` from `grep`'s output
```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{oDX0uYlJhf8lLmaTvtr-z-_DXx9.0FOxEzNxwiMwAzNzEzW}
```

## Flag
`pwn.college{oDX0uYlJhf8lLmaTvtr-z-_DXx9.0FOxEzNxwiMwAzNzEzW}`
### Notes
- the `-v` argument for `grep` _inverts_ its filters, i.e. turning `grep` from a _whitelist_ to a _blacklist_