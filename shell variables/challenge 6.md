# **SHELL VARIABLES**
## **<ins>STORING COMMAND OUTPUT</ins>**
Using command substitution we can store the output of some command into a variable.

### SOLVE: 
***FLAG:*** pwn.college{saQ-BzZCRzsJQB-h9oDXeaelv8I.QX1cDN1wSO2kjNzEzW}

I first used the command PWN=$(/challenge/run) which stored the flag in the PWN variable. The flag was initially stored in /challenge/run.
Now we use the echo command to print the flag which is stored in the variable. 

```
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{saQ-BzZCRzsJQB-h9oDXeaelv8I.QX1cDN1wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about storing the command output in a variable and how to access it.

### REFERENCES:
None.
