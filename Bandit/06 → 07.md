# Level Goal

The password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size

# Solution
It says stored somewhere on the server. So I have to search the whole root directory. We have to use the `find` command with `-user`, `-group` and `-size` flags.

```
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```

The `2>/dev/null` redirects standard error output.
