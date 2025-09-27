# **DIGESTING DOCUMENTATION**
## **<ins>READING MANUALS</ins>**
I learnt how to use the man command to read the manual of the command that is passed as an argument.

### SOLVE: 
***FLAG:*** pwn.college{kIM9jrBaf_h-zLOBnN7oZf9iY_N.QX0EDO0wSO2kjNzEzW}

Here I learnt about the manual command that is man, hence using the man command on the challenge argument. man challenge.
The manual page of challenge pops up.
In the description of this page there is a line mentioned, 
 Output the flag when called with the right arguments.
  --kjrafh NUM
              print the flag if NUM is 979
Hence by using the command /challenge/challenge --kjrafh 979 we obtain the flag.

```
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --kjrafh 979
Correct usage! Your flag: pwn.college{kIM9jrBaf_h-zLOBnN7oZf9iY_N.QX0EDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to use the manual command that is man and what the use of this command is.

### REFERENCES:
None.


 
