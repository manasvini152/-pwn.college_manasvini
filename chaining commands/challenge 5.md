# **CHAINING COMMANDS**
## **<ins>REDIRECTING SCRIPT OUTPUT</ins>**
We add two files to the shell script and execute them using another file using piping and bash command.

### SOLVE: 
***FLAG:*** pwn.college{YeHLyCXLDCspDG7z5XIQD6pwnsT.QX4ETO0wSO2kjNzEzW}

I added the two files in the shell as I did in the previous challenge. I then piped out the output to /challenge/solve
using the bash command.

```
hacker@chaining~redirecting-script-output:~$ echo '/challenge/pwn ; /challenge/college' > x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{YeHLyCXLDCspDG7z5XIQD6pwnsT.QX4ETO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
To send the output of several programs to one command using piping command.

### REFERENCES:
None. 
