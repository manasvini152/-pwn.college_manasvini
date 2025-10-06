# **PROCESSES AND JOBS**
## **<ins>INTERRUPTING PROCESSES</ins>**
The Ctrl+C command sends an interrupt to the application which is waiting on an input. This causes the application to exit.

### SOLVE: 
***FLAG:*** pwn.college{sOt0L_SBhPNqSe5o1UxjRRqvSXF.QXzQDO0wSO2kjNzEzW}

By running the command /challenge/run the flag is not obtained since the terminal is waiting on an input.
Now by using Ctrl+C the flag is obtained as the application is exited.


```
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{sOt0L_SBhPNqSe5o1UxjRRqvSXF.QXzQDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to interrupt an application using the keys Ctrl+C.

### REFERENCES:
None.
