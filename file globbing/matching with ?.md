# **FILE GLOBBING**
## **<ins>MATCHING WITH ?</ins>**
I learnt about the globbing operator ?. The shell treats it as a single character.

### SOLVE: 
***FLAG:*** pwn.college{Ilt3u7qsxseHLf5Fdc_L_5hqvuN.QXyIDO0wSO2kjNzEzW}

I ran the  cd /?ha??enge which replaced the characters c and l with the ?.
Hence the directory was changed to /challenge. 
Then I ran the command /challenge/run which gave me the flag.

```
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{Ilt3u7qsxseHLf5Fdc_L_5hqvuN.QXyIDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the globbing operator ?, which replaces one character.

### REFERENCES:
None.
