# **DATA MANIPULATION**
## **<ins>DELETING CHARACTERS</ins>**
We can delete a character using the tr -d command.

### SOLVE: 
***FLAG:*** pwn.college{w8V2jFN_p6aNipPM7DpJF-YnKfZ.0FNxEzNxwSO2kjNzEzW}

By using the command /challenge/run | tr -d ^% we delete the characters ^ and % from the flags. Hence we obtain the flag.

```
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{w8V2jFN_p6aNipPM7DpJF-YnKfZ.0FNxEzNxwSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the tr -d command which replaces characters with nothing or deletes characters.

### REFERENCES:
None. 
