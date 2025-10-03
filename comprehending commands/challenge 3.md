# **COMPREHENDING COMMANDS**
## **<ins>MORE CATTING PRACTICE</ins>**
Here the file exists in another directory which needs to be accessed without using the cd command.
### SOLVE: 
***FLAG:*** pwn.college{kB4VeFFmx0ovXPHfbFWK-Z7ftOH.QXwITO0wSO2kjNzEzW}

When we connect via the ssh key we get a message that says the cd command cannot be used in this level, and that the flag must be retrieved 
with the help of an absolute path. The file the flag is in is mentioned which is /lib/bash/flag.
Therefore we can cat it without changing the directories by using an absolute path using the command cat /lib/bash/flag
Hence we obtain the flag.
```
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /lib/bash/flag. Go cat it out **without** cding into that directory!
hacker@commands~more-catting-practice:~$ cat /lib/bash/flag
pwn.college{kB4VeFFmx0ovXPHfbFWK-Z7ftOH.QXwITO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to access a file without changing directories, and by using an absolute path.

### REFERENCES:
None.
