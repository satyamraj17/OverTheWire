# Level Goal
The password for the next level is stored in a file called - located in the home directory

# Solution
The file name is `-`. Using `cat -` won't work, because the binary treats it as a flag and expects it. Using single quotes will also not work. The best way to read it is using a relative path `./-`
```
bandit1@bandit:~$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```
