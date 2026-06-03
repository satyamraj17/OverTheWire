# Level Goal

The password for the next level is stored in the file data.txt next to the word millionth

# Solution
We have to use `grep` here. We will target the word `millionth`, and it will print the line containing the word.
```
bandit7@bandit:~$ grep millionth data.txt 
millionth       dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```
