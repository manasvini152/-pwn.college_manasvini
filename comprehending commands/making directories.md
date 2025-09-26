# **COMPREHENDING COMMANDS**
## **<ins>MAKING DIRECTORIES</ins>**
We learn how to create a new directory using the mkdir command.

### SOLVE: 
***FLAG:*** pwn.college{8knyVzZ_OKzqkdbB0fgY_3wWks5.QXxMDO0wSO2kjNzEzW}

The directory to be created was given as /tmp/pwn, I created the directory using the mkdir command hence used the command mkdir /tmp/pwn.
Then I switched the directories to the new directory created using the cd command, cd /tmp/pwn.
Then the question asked to create a new file named college which I did using the touch command. touch college
Hence by entering the /challenge/run command I obtained the flag.

```
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{8knyVzZ_OKzqkdbB0fgY_3wWks5.QXxMDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to create a new directory using the mkdir command and create a new file in the directory using the touch command.

### REFERENCES:
None.
