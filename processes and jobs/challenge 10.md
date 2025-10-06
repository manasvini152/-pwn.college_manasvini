# **PROCESSES AND JOBS**
## **<ins>PROCESS EXIT CODES</ins>**
Every program exits with an exit code when it finishes running and terminates.

### SOLVE: 
***FLAG:*** pwn.college{w-qRo9rUqznwUiMbMTJS-bMOPDV.QX5YDO1wSO2kjNzEzW}

By running the command /challenge/get-code and then by running the command echo $?.
We get the error code. Then we run the /challenge/submit-code command along with the error code as the argument.

```
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
162
hacker@processes~process-exit-codes:~$ /challenge/submit-code 162
CORRECT! Here is your flag:
pwn.college{w-qRo9rUqznwUiMbMTJS-bMOPDV.QX5YDO1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the exit code and which finishes runnning and terminates the program. 

### REFERENCES:
None. 
