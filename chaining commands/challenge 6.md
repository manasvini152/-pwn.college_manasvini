# **CHAINING COMMANDS**
## **<ins>EXECUTABLE SHELL SCRIPTS</ins>**
We invoke /challenge/solve and make it executable and we run it without using bash.

### SOLVE: 
***FLAG:*** pwn.college{0KVh0iy-y1aDDN8O_QTCaw2NwbH.QX0cjM1wSO2kjNzEzW}

I used the echo command to invoke /challenge/solve with the help of the shell script. 
Then I used chmod command to give executable access to x.sh. Then by running the command ./x.sh.

```
hacker@chaining~executable-shell-scripts:~$ echo /challenge/solve > x.sh
hacker@chaining~executable-shell-scripts:~$ chmod a+x x.sh
hacker@chaining~executable-shell-scripts:~$ ./x.sh
Congratulations on your shell script execution! Your flag:
pwn.college{0KVh0iy-y1aDDN8O_QTCaw2NwbH.QX0cjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
To execute shell script without using the bash command. 

### REFERENCES:
None. 
