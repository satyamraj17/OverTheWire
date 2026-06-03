# Level Goal

The password for the next level is stored in a hidden file in the inhere directory.

# Solution

Just like the previous task, use the relative path, then press Tab to see the file name.
```
bandit3@bandit:~$ cat inhere/...Hiding-From-You 
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```

We can also use the `ls -a` command to list the hidden files, and then using the `cat` command to show the content of the file.
```
bandit3@bandit:~$ ls -a inhere/
.  ..  ...Hiding-From-You
bandit3@bandit:~$ cat inhere/...Hiding-From-You 
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```
