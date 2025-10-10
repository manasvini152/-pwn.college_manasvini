# **CHAINING COMMANDS**
## **<ins>HANDLING FAILURE</ins>**
The || operator runs the second command only if the first command fails.

### SOLVE: 
***FLAG:*** pwn.college{YNt2o6KCKpF9xmT_EdF7YeVS7Wz.01M0MDOxwSO2kjNzEzW}

In this challenge /challenge/first-failure and /challenge/second do not run individually and only gives the flag when chained using the
|| operator.

```
hacker@chaining~handling-failure:~$ /challenge/first-failure || /challenge/second
Nice chaining! Flag: pwn.college{YNt2o6KCKpF9xmT_EdF7YeVS7Wz.01M0MDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to chain commands using the || operator. 

### REFERENCES:
None. 
