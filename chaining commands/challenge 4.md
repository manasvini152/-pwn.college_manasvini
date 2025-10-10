# **CHAINING COMMANDS**
## **<ins>YOUR FIRST SHELL SCRIPT</ins>**
We are supposed run /challenge/pwn and /challenge/college in a shell script x.sh.

### SOLVE: 
***FLAG:*** pwn.college{kxYG0dOnfeMa75livGq2D7rnIT3.QXxcDO0wSO2kjNzEzW}

We put these commands in a file called shell script. We create a shell script called x.sh.

```
hacker@chaining~your-first-shell-script:~$ echo '/challenge/pwn;/challenge/college' > x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{kxYG0dOnfeMa75livGq2D7rnIT3.QXxcDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to make a shell script and execute it.

### REFERENCES:
None. 
