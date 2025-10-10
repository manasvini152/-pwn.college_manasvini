# **CHAINING COMMANDS**
## **<ins>BUILDING ON SUCCESS</ins>**
The && operator allows us to run the second command only if the first one is executed.

### SOLVE: 
***FLAG:***  pwn.college{AigaB34bnxBqSvTx6nCkzslDgnQ.0lM0MDOxwSO2kjNzEzW}

The command /challenge/first-success and the command /challenge/second does not work
individually and needs to be chained using the && operator. 

```
hacker@chaining~building-on-success:~$ /challenge/first-success
hacker@chaining~building-on-success:~$ /challenge/second
Error: /challenge/first-success must be successfully chained with
/challenge/second using &&
hacker@chaining~building-on-success:~$ /challenge/first-success && /challenge/second
Nice chaining! Flag: pwn.college{AigaB34bnxBqSvTx6nCkzslDgnQ.0lM0MDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to chain commands using the && operator. 

### REFERENCES:
None. 
