# **SHELL VARIABLES**
## **<ins>READING INPUT</ins>**
We use the read builtin to input values to a variable.

### SOLVE: 
***FLAG:*** pwn.college{cssPWAgnWW7HI3q1kYAa3__AnFN.QX4cTN0wSO2kjNzEzW}

By using the command read PWN, the users can input a value that will be stored in the variable PWN.
As the challenge requires we enter the value COLLEGE and hence we obtain the flag.

```
hacker@variables~reading-input:~$ read PWN
COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{cssPWAgnWW7HI3q1kYAa3__AnFN.QX4cTN0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the read command. That allows the users to enter the values.

### REFERENCES:
None.
