# **COMPREHENDING COMMANDS**
## **<ins>LINKING FILES</ins>**
We learn how to link files using the ln -s command.

### SOLVE: 
***FLAG:***  pwn.college{EpWD8D4cL3TWaF7dbhigSO0QVZx.QX5ETN1wSO2kjNzEzW}

Using the linking command, I created a symbolic link between the /flag and /home/hacker/not-the-flag command.
Then by invoking the /challenge/catflag command we get the flag.

```
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{EpWD8D4cL3TWaF7dbhigSO0QVZx.QX5ETN1wSO2kjNzEzW}
```

### WHAT I LEARNED:  
I learnt about symbolic links using the ln -s command. Link is used when two programs want to access the same data from different locations.

### REFERENCES:
None.
