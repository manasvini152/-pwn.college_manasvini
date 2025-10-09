# **PERCEIVING PERMISSIONS**
## **<ins>GROUPS AND FILES</ins>**
We use the chgrp command to change the group ownership.

### SOLVE: 
***FLAG:*** pwn.college{gUtukFALqAb79QSt5RAt1OhejUd.QXxcjM1wSO2kjNzEzW}

By using the command chgrp hacker /flag we change the group ownership to hacker. And I read the flag file by using the cat command
and obtained the flag.

```
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{gUtukFALqAb79QSt5RAt1OhejUd.QXxcjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the chgrp command and how to use the command to change group ownership. 

### REFERENCES:
None. 
