# **COMPREHENDING COMMANDS**
## **<ins>CATTING ABSOLUTE PATHS</ins>**
In the previous challenge we accessed the file flag directly from the home directory, here we read the file as an absolute path.
### SOLVE: 
***FLAG:*** pwn.college{MCTinAb1wWDUuRfVPP_S3vA81rm.QX5ETO0wSO2kjNzEzW}

The command cat flag does not work here since the file flag does not exist in the home directory.
Hence we need to invoke an absolute path by using the / command.
When we enter cat /flag we can obtain the flag with the help of an absolute path.

```
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{MCTinAb1wWDUuRfVPP_S3vA81rm.QX5ETO0wSO2kjNzEzW}
hacker@commands~catting-absolute-paths:~$ cat flag
cat: flag: No such file or directory
```

### WHAT I LEARNED:  
I learnt how to access a file with the help of an absolute path through a cat command.

### REFERENCES:
None.
