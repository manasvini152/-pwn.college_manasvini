# **COMPREHENDING COMMANDS**
## **<ins>LISTING FILES</ins>**
We learn about the listing files ls command. Which lists the contents in a directory.
### SOLVE: 
***FLAG:***  pwn.college{UaYNPrpA3hn7T2lSIw08zdt9Yxp.QX4IDO0wSO2kjNzEzW}

First I tried to list the contents in /challenge using the ls command, which gave me a name 17744-renamed-run-17575. 
Now since we got the file in the directory challenge we use the command /challenge/17744-renamed-run-17575 to obtain the flag.

```
hacker@commands~listing-files:~$ ls /challenge
17744-renamed-run-17575  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/17744-renamed-run-17575
Yahaha, you found me! Here is your flag:
pwn.college{UaYNPrpA3hn7T2lSIw08zdt9Yxp.QX4IDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:  
I learnt about the ls command and how to list the contents in a particular directory. 

### REFERENCES:
None.
