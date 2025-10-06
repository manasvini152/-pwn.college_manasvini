# **PROCESSES AND JOBS**
## **<ins>FOREGROUNDING PROCESSES</ins>**
We can use the fg command to resume a process which has been running in the background.

### SOLVE: 
***FLAG:*** pwn.college{cFu70xX7weXnc-g_Z_NQveImJOb.QX4QDO0wSO2kjNzEzW}

I ran the command /challenge/run and then suspended the process using Ctrl+Z. Then I ran the process in the background by using 
the bg command. Then I resumed the background process by using the fg command and obtained the flag.


```
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~foregrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.

hacker@processes~foregrounding-processes:~$ fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{cFu70xX7weXnc-g_Z_NQveImJOb.QX4QDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt that a background process can be resumed by using the fg command.

### REFERENCES:
None. 
