# **PRACTICING PIPING**
## **<ins>WRITING TO MULTIPLE PROGRAMS</ins>**
Using the >(command) operator we obtain the flag. Which is output process substitution. 

### SOLVE: 
***FLAG:*** pwn.college{YQGHiVgz7SQKQIF8Gyx95-gcKBE.QXwgDN1wSO2kjNzEzW}

By using the command /challenge/hack | tee >(/challenge/the) >(/challenge/planet), we run the /challenge/hack command and 
and duplicate the output into the /challenge/the and /challenge/planet command. We use output process substitution >(command).
We use the tee command to dupliate the data.

```
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
10566254421797520681
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{YQGHiVgz7SQKQIF8Gyx95-gcKBE.QXwgDN1wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about output process substituion and how to duplicate data using the tee command. I also learnt about the syntax for output 
process substitution.

### REFERENCES:
None.
