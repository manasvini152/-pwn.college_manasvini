# **DATA MANIPULATION**
## **<ins>TRANSLATING CHARACTERS</ins>**
tr translates the character provided in the first argument to the character provided in the second argument.

### SOLVE: 
***FLAG:*** pwn.college{IGeAGOmHbxKRrQRhdRqjtZ6lHzM.01MxEzNxwSO2kjNzEzW}

I ran the command /challenge/run | tr a-zA-Z A-Za-z which swapped the characters a-z with the characters of A-Z. 
Which also swaps the characters A-Z with the characters a-z. Using the tr command.

```
hacker@data~translating-characters:~$ /challenge/run | tr a-zA-Z A-Za-z
yOUR CASE-SWAPPED FLAG:
pwn.college{IGeAGOmHbxKRrQRhdRqjtZ6lHzM.01MxEzNxwSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt the use of the tr command which swaps the characters.

### REFERENCES:
None. 
