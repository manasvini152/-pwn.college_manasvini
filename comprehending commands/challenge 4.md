# **COMPREHENDING COMMANDS**
## **<ins>GREPPING FOR A NEEDLE IN A HAYSTACK</ins>**
When we file we cat out is too big we need to use the grep command to search for a particular content in the file.
### SOLVE: 
***FLAG:*** pwn.college{YPZM6rwuELVdmhlo8DBGZSe56XT.QX3EDO0wSO2kjNzEzW}

If we enter cat /challenge/data.txt like we did in the previous challenged it will provide a long list of contents which makes it almost 
impossible to find the flag.
Hence we use the grep command which helps us search content.
The syntax for the grep command is ```grep SEARCH_STRING /path/to/file``` 
The file name is /challenge/data.txt and we know that the flag starts with pwn.college, hence the command will be
grep pwn.college /challenge/data.txt and hence we obtain the flag.

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{YPZM6rwuELVdmhlo8DBGZSe56XT.QX3EDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the grep command and how to use it. I learnt how to search for a particular content with the help of grep command in a 
particular file.

### REFERENCES:
None.
