# **SHELL VARIABLES**
## **<ins>EXPORTING VARIABLES</ins>**
We use the export command to obtain the flag.

### SOLVE: 
***FLAG:*** pwn.college{Yy21jIq7Q7_XLS5U-JaEmtFG6E2.QXyYTN0wSO2kjNzEzW}

The challenge tells us to invoke /challenge/run when the PWN variable is exported and
value is set to COLLEGE. And it asks us to set the value of the variable COLLEGE to PWN,
without exporting it. Hence I used the commands export PWN=COLLEGE and COLLEGE=PWN.
After doing this I ran the command /challenge/run the flag was displayed.

```
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{Yy21jIq7Q7_XLS5U-JaEmtFG6E2.QXyYTN0wSO2kjNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

### WHAT I LEARNED: 
I learnt about the export command and how to assign values to variables using this command.

### REFERENCES:
None.
