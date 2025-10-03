# **FILE GLOBBING**
## **<ins>MULTIPLE GLOBS</ins>**
Bash supports multiple globs at once in a single word.

### SOLVE: 
***FLAG:*** pwn.college{wrG1ad3JEZps6XnwNOHKRZMweWW.0lM3kjNxwSO2kjNzEzW}

First I changed the directories to /challenge/files using the cd command.
Then I used the command /challenge/run command along with an argument that 
matched the conditions required that is two globs and the letter p.
By invoking this command the flag is obtained.

```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{wrG1ad3JEZps6XnwNOHKRZMweWW.0lM3kjNxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to execute multiple glob commands at one time.

### REFERENCES:
None.

