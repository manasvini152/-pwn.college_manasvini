# **PROCESSES AND JOBS**
## **<ins>SUSPENDING PROCESSES</ins>**
The Ctrl+Z command suspends the process to the background. 

### SOLVE: 
***FLAG:*** pwn.college{kn594zHjEiryZ6VnuNnTc5Ss2Bw.QX1QDO0wSO2kjNzEzW}

By running the command /challenge/run we do not get the flag since the challenge requires two copies of the process running.
But in order to run the second copy we must suspend the first copy, we do this by running the key Ctrl+Z.
Hence by running /challenge/run again we obtain the flag.


```
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         138     129  0 20:29 pts/0    00:00:00 bash /challenge/run
root         140     138  0 20:29 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         138     129  0 20:29 pts/0    00:00:00 bash /challenge/run
root         145     129  0 20:29 pts/0    00:00:00 bash /challenge/run
root         147     145  0 20:29 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{kn594zHjEiryZ6VnuNnTc5Ss2Bw.QX1QDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to suspend a process by running the command key Ctrl+Z.

### REFERENCES:
None. 
