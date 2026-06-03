# Level Goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable

# Solution

We need to find the file that satisfies the 3 conditions. We can use the `find` command for this.
```
bandit5@bandit:~/inhere$ find . -size 1033c \! -executable
./maybehere07/.file2
bandit5@bandit:~/inhere$ file ./maybehere07/.file2
./maybehere07/.file2: ASCII text, with very long lines (1000)
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```
