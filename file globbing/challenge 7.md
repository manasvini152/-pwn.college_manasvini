# **FILE GLOBBING**
## **<ins>EXCLUSIONARY GLOBBING</ins>**
To filter out files in the glob, using the ! or ^ operator. 

### SOLVE: 
***FLAG:*** pwn.college{8YMZesAUt3UJtcV3eOxrLz8fetX.QX2IDO0wSO2kjNzEzW}

First I changed the directory to /challenge/files using the cd command.
Then I used the /challenge/run and the inverter command for the characters p,w and n.
Once this command is invoked then the flag is displayed.

```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]*
You got it! Here is your flag!
pwn.college{8YMZesAUt3UJtcV3eOxrLz8fetX.QX2IDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to filter out characters in the glob, using the inverter operator.

### REFERENCES:
None.
