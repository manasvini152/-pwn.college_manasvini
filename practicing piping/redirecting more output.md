# **PRACTICING PIPING**
## **<ins>REDIRECTING MORE OUTPUT</ins>**
Redirecting the output without using echo and redirecting the output of any command.

### SOLVE: 
***FLAG:*** pwn.college{MxWgLjnxrHc9Z2Oi81PtQg5HI7J.QX1YTN0wSO2kjNzEzW}

I first used the command /challenge/run > myflag which redirects the /challenge/run output to the file 
myflag. After the output is redirected to the file myflag I catted out the file.
Using the cat myflag command the flag was displayed.

```
hacker@piping~redirecting-more-output:~$  /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{MxWgLjnxrHc9Z2Oi81PtQg5HI7J.QX1YTN0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to redirect the output to a file without using the echo and obtaining the file using the cat command.

### REFERENCES:
None.
