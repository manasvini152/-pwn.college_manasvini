# **PRACTICING PIPING**
## **<ins>REDIRECTING ERRORS</ins>**
We can redirect errors using the command 2> which is under the file descriptor.

### SOLVE: 
***FLAG:***  pwn.college{wxlVWJ0Q8jfc0H0WoGRiTlyuc9l.QX3YTN0wSO2kjNzEzW}

I first executed the command /challenge/run > myflag 2> instructions which is the syntax to redirect multiple command at once.
Where the output of /challenge/run is being redirected to myflag and the error of /challenge/run is being redirected to instructions.
Once this is done we can cat out the files to get the desired output. Once we cat out the instructions file we get feedback or comments.
And once we cat out the myflag command we get the flag.

```
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{wxlVWJ0Q8jfc0H0WoGRiTlyuc9l.QX3YTN0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to redirect errors. I learnt about the three file descriptor (FD) commands. 
That is the standard input, standard output and the standard error commands.

### REFERENCES:
None.
