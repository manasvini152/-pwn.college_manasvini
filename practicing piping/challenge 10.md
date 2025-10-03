# **PRACTICING PIPING**
## **<ins>DUPLICATING PIPED DATA WITH TEE</ins>**
We use the tee command that executes and saves the output of more than one command at once.

### SOLVE: 
***FLAG:*** pwn.college{wuz-p4KndEoqTwfbrzKoquA9ug6.QXxITO0wSO2kjNzEzW}

By using the command /challenge/pwn | tee pwn | /challenge/college, we pipe /challenge/pwn into /challenge/college.
We tee the output to save the output of /challenge/pwn. Then we cat out the variable PWN which gives us a secret code.
The secret code is supposed to be used with /challenge/pwn hence we use the command /challenge/pwn --secret wuz-p4Kn |  /challenge/colleg.
Which gives us the flag.

```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pwn | /challenge/college
Processing...
WARNING: you are overwriting file pwn with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "wuz-p4Kn"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret wuz-p4Kn |  /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{wuz-p4KndEoqTwfbrzKoquA9ug6.QXxITO0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the tee command and the use of the tee command two read and output different commands.

### REFERENCES:
None.
