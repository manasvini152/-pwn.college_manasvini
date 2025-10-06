# **PROCESSES AND JOBS**
## **<ins>STARTING BACKGROUNDED PROCESSES</ins>**
To run processes in the background it need not be suspended. We can do this by using the append command &.

### SOLVE: 
***FLAG:*** pwn.college{oMs2x5fynS3iUXH5sbcPDW6XtXj.QX5QDO0wSO2kjNzEzW}

By running the command /challenge/run &, we run the process in the background without needing to suspend it.

```
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[2] 146
hacker@processes~starting-backgrounded-processes:~$


Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{oMs2x5fynS3iUXH5sbcPDW6XtXj.QX5QDO0wSO2kjNzEzW}

[2]+  Done                    /challenge/run
```

### WHAT I LEARNED:
We can run a process in the background without needing to suspend it using the & command.

### REFERENCES:
None. 
