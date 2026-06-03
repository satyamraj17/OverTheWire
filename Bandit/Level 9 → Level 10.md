# Level Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

# Solution
Using `strings` to print the printable/human-readable strings in the file, and then using `grep` to find the lines with '=' in them.
```
bandit9@bandit:~$ strings data.txt | grep '=========='
 ========== the
========== password
========== is
========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```
