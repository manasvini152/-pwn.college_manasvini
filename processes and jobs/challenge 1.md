# **PROCESSES AND JOBS**
## **<ins>LISTING PROCESSES</ins>**
the ps command lists processes running in the terminal. 
ps aux lists all the running processes on the system along with other information.

### SOLVE: 
***FLAG:*** pwn.college{Upkl4frUpvHZDKhWQwt7N22oMPn.QX4MDO0wSO2kjNzEzW}

By running the command ps aux we get a list of all the runnning processes. Since there is no directory called /challenge/run.
But there is a directory named /challenge/908-run-30405 which gives us the flag when invoked.

```
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.2  0.0   1056   640 ?        Ss   19:32   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.1  0.0 231708  2560 ?        S    19:32   0:00 /run/dojo/bin/sleep 6h
root         132  0.0  0.0   4132  2560 ?        S    19:32   0:00 /challenge/908-run-30405
root         135  0.0  0.0   2744  1600 ?        S    19:32   0:00 sleep 6h
hacker       137  0.9  0.0 231576  3520 pts/0    Ss   19:32   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       143  0.0  0.0 231940  4160 pts/0    S    19:32   0:00 /run/dojo/bin/bash --login
hacker       152  0.0  0.0 233600  3840 pts/0    R+   19:32   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/908-run-30405
Yahaha, you found me! Here is your flag:
pwn.college{Upkl4frUpvHZDKhWQwt7N22oMPn.QX4MDO0wSO2kjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```

### WHAT I LEARNED:
I learnt about the ps command along with the ps -ef and ps aux command.

### REFERENCES:
None. 

