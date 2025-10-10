# **PONDERING PATH**
## **<ins>FINDING COMMANDS</ins>**

We use the which command.

### SOLVE: 
***FLAG:***  pwn.college{IxOQ-wMIOhR9DOaI_Ntf1iNnoEU.01NzEzNxwSO2kjNzEzW}

By using the command which win we get a directory and hence by catting out the directory with the help of the flag file we obtain the flag.

```
hacker@path~finding-commands:~$ which win
/challenge/paths/4335/win
hacker@path~finding-commands:~$ cat /challenge/paths/4335/flag
pwn.college{IxOQ-wMIOhR9DOaI_Ntf1iNnoEU.01NzEzNxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the which command which looks at each directory in the PATH.

### REFERENCES:
None. 
