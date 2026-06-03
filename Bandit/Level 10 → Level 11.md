# Level Goal

The password for the next level is stored in the file data.txt, which contains base64 encoded data

# Solution
The file contains base64-encoded data. We only have to decode it using `base64`.
```
bandit10@bandit:~$ cat data.txt | base64 -d
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```
