# **PERCEIVING PERMISSIONS**
## **<ins>CHANGING FILE OWNERSHIP</ins>**
We use the chown command to change the ownership of the file.

### SOLVE: 
***FLAG:*** pwn.college{039iYb-8RPRm7lsHVP3HBo6_lzl.QXxEjN0wSO2kjNzEzW}

By using the command chown hacker /flag, we give the user hacker permission to access the file /flag. 
Then by reading the file by using the cat command we obtain the flag. The hacker user had all the permissions. 

```
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{039iYb-8RPRm7lsHVP3HBo6_lzl.QXxEjN0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the chown command, which is the change ownership command. 

### REFERENCES:
None. 
