# Level Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

# Solution
We need to find the word with a count of 1. Sort the data using `sort`, then use `uniq` to find the `uniq` to find the unique entry.
```
bandit8@bandit:~$ sort data.txt | uniq -u
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```
