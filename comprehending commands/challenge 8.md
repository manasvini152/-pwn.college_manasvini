# **COMPREHENDING COMMANDS**
## **<ins>REMOVING FILES</ins>**
We learn how to remove files using the rm command.

### SOLVE: 
***FLAG:*** pwn.college{00zr6dYP0PzOwmci7ZHH-0R4Hin.QX2kDM1wSO2kjNzEzW}

First I used the ls command to check the files in the home directory. It showed two files including the one to be removed.
Then I used the remove command rm to remove the file delete_me.
Once deleted I ran the command /challenge/check to obtain the flag.

```
hacker@commands~removing-files:~$ ls
delete_me  m
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{00zr6dYP0PzOwmci7ZHH-0R4Hin.QX2kDM1wSO2kjNzEzW}
hacker@commands~removing-files:~$ ls
m
```

### EXTRA:
```
hacker@commands~removing-files:~$ touch delete_me
hacker@commands~removing-files:~$ ls
delete_me  m
hacker@commands~removing-files:~$ /challenge/check
It looks like /home/hacker/delete_me still exists! rm it.
```

### WHAT I LEARNED:  
I learnt how to remove a file from a directory using the rm command.

### REFERENCES:
None.
