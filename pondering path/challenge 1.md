# **PONDERING PATH**
## **<ins>THE PATH VARIABLE</ins>**

We remove the path to rm command so that the flag does not get deleted from /challenge/run.

### SOLVE: 
***FLAG:*** pwn.college{I6PKeEieLTbbDMBITckKoftQN2K.QX2cDM1wSO2kjNzEzW}

I used the command PATH="" which removed the path variable. And hence by running /challenge/run we obtain the flag.

```
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{I6PKeEieLTbbDMBITckKoftQN2K.QX2cDM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to remove the path variable.

### REFERENCES:
None. 
