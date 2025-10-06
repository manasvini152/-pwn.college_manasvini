# **PROCESSES AND JOBS**
## **<ins>BACKGROUNDING PROCESSES</ins>**
Instead of resuming the suspended processes we can run the process in the background using the bg command.
This command allows the process to run in the background while other commands can be invoked.

### SOLVE: 
***FLAG:*** pwn.college{oNd3HJNqmATcnUEb7Jm48YXFg2k.QX3QDO0wSO2kjNzEzW}

By running the command /challenge/run and suspending the process using the Ctrl+Z key. Then I ran the process in the background by 
using the bg command. And now we execute /challenge/run again while the first one is running in the background to get the flag.


```
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         138 S+   bash /challenge/run
root         140 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~backgrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         138 S    bash /challenge/run
root         148 S    sleep 6h
root         149 S+   bash /challenge/run
root         151 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{oNd3HJNqmATcnUEb7Jm48YXFg2k.QX3QDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to run a process in the background by using the bg command.

### REFERENCES:
None. 
