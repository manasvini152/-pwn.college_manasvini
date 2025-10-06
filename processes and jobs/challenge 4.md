# **PROCESSES AND JOBS**
## **<ins>KILLING MISBEHAVING PROCESSES</ins>**
A named pipe FIFO has a bunch of decoy flags and this process needs to be killed.

### SOLVE: 
***FLAG:*** pwn.college{MCd8yr0AWJXQOvy7P4kb4aoc9zA.0FNzMDOxwSO2kjNzEzW}

I ran the command ps aux first which gave me the list of processes running and hence I used the kill command on the /challenge/decoy
process. Now by running the command /challenge/run the flag is sent to /tmp/flag_fifo. Then we use the Ctrl+C key and then I catted out
/tmp/flag_fifo which gave a bunch of decoy flags and had to use the Ctrl+C key. By running the /challenge/run and catting out /tmp/flag_fifo
again we obtain the flag.

```
hacker@processes~killing-misbehaving-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.4  0.0   1056   640 ?        Ss   20:22   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.3  0.0 231708  2560 ?        S    20:22   0:00 /run/dojo/bin/sleep 6h
root         137  0.0  0.0   4132  1280 ?        S    20:22   0:00 /bin/bash /challenge/.init
root         138  0.0  0.0   4132  1280 ?        S    20:22   0:00 /bin/bash /challenge/.init
root         139  0.0  0.0   5204  3520 ?        S    20:22   0:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         140  0.0  0.0   2744  1600 ?        S    20:22   0:00 sleep 6h
root         141  0.0  0.0   2744  1600 ?        S    20:22   0:00 sleep 6h
hacker       142  0.4  0.0  13516  9280 ?        Ss   20:22   0:00 /usr/bin/python /challenge/decoy
hacker       144  0.9  0.0 231576  3520 pts/0    Ss   20:22   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       150  0.0  0.0 231972  4160 pts/0    S    20:22   0:00 /run/dojo/bin/bash --login
hacker       159  0.0  0.0 233600  3840 pts/0    R+   20:22   0:00 ps aux
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
^C
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{MCd8yr0AWJXQOvy7P4kb4aoc9zA.0FNzMDOxwSO2kjNzEzW}
y7P4kb4aoc9zA.0FNzMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to find a flag among a bunch of decoy flags using the kill command.

### REFERENCES:
None. 
