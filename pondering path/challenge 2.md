# **PONDERING PATH**
## **<ins>SETTING PATH</ins>**

We set the PATH to a directory.

### SOLVE: 
***FLAG:*** pwn.college{4Ngq5K_neKnrTVmllo37GiBg0tq.QX1cjM1wSO2kjNzEzW}

By overwriting PATH with the directory /challenge/more_commands/, we run /challenge/run which gives us the flag.

```
hacker@path~setting-path:~$ PATH='/challenge/more_commands/'
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{4Ngq5K_neKnrTVmllo37GiBg0tq.QX1cjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to set the PATH.

### REFERENCES:
None. 
