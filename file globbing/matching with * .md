# **FILE GLOBBING**
## **<ins>MATCHING WITH '*'</ins>**
I learnt about globbing and what the * operator does. The shell replaces * with any argument that matches the pattern.

### SOLVE: 
***FLAG:*** pwn.college{YjRx89-fufhYO_CcNXvTqvIKvIQ.QXxIDO0wSO2kjNzEzW}

I ran the cd /ch* command which globbed the cd /challenge command, once it changed directories to /challenge.
Then I ran the /challenge/run command which gave me the flag.

```
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{YjRx89-fufhYO_CcNXvTqvIKvIQ.QXxIDO0wSO2kjNzEzW}

```

### WHAT I LEARNED: 
I learnt about globbing and how the * operator replaces arguments with similar patterns.

### REFERENCES:
None.
