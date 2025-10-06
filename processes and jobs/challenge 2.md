# **PROCESSES AND JOBS**
## **<ins>KILLING PROCESSES</ins>**
The kill command terminates a process. We use a process identifier along with the kill command.

### SOLVE: 
***FLAG:*** pwn.college{cJmb45piT18MvZr_qp_w7Qf2vmz.QXyQDO0wSO2kjNzEzW}

The /challenge/run command will not execute as /challenge/dont_run is still running. Hence we have to terminate /challenge/dont_run.
In order to kill the process we need a process identifier which we obtain by using the command ps aux.
After executing the ps aux command we get the process identifier as 136 for /challenge/dont_run and by using the command kill 136.
/challenge/dont_run is terminated. Hence now we run /challenge/run and obtain the flag.

```
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   19:45   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.0  0.0 231708  2560 ?        S    19:45   0:00 /run/dojo/bin/sleep 6h
root         135  0.0  0.0   5204  3200 ?        S    19:45   0:00 su -c /challenge/.launcher hacker
hacker       136  0.0  0.0 231576  3520 ?        Ss   19:45   0:00 /challenge/dont_run
hacker       137  0.0  0.0 231708  2560 ?        S    19:45   0:00 sleep 6h
hacker       139  0.0  0.0 231576  3520 pts/0    Ss   19:45   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       145  0.0  0.0 231940  4160 pts/0    S    19:45   0:00 /run/dojo/bin/bash --login
hacker       159  0.0  0.0 233600  3840 pts/0    R+   19:46   0:00 ps aux
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{cJmb45piT18MvZr_qp_w7Qf2vmz.QXyQDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to terminate a process using the kill command and the process identifier of that particular process.

### REFERENCES:
None. 
