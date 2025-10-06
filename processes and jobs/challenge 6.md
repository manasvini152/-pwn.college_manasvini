# **PROCESSES AND JOBS**
## **<ins>RESUMING PROCESSES</ins>**
After suspending a process we can resume it by running the fg command.

### SOLVE: 
***FLAG:*** pwn.college{88ocA9W13LiAniQVoxcSD52DAZ3.QX2QDO0wSO2kjNzEzW}

I first ran the command /challenge/run and then suspended the process by using Ctrl+Z and then resumed the process by using 
the fg command which gave us the flag.

```
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{88ocA9W13LiAniQVoxcSD52DAZ3.QX2QDO0wSO2kjNzEzW}
Don't forget to press Enter to quit me!

Goodbye!
```

### WHAT I LEARNED:
I learnt how to resume a suspended process using the fg command.

### REFERENCES:
None. 
