# **PERCEIVING PERMISSIONS**
## **<ins>EXECUTABLE FILES</ins>**
We use the chmod command to make /challenge/run executable. 

### SOLVE: 
***FLAG:***  pwn.college{8UeUxncJ6BQ5Q3mcTPFL0-ydTk9.QXyEjN0wSO2kjNzEzW}

We use the command chmod a+x /challenge/run where all the users groups and other users are executable. 
Once this permission is granted we use the command /challenge/run to get the flag.

```
hacker@permissions~executable-files:~$ chmod a+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{8UeUxncJ6BQ5Q3mcTPFL0-ydTk9.QXyEjN0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to make a file executable by using the chmod command.

### REFERENCES:
None. 
