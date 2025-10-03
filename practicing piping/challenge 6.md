# **PRACTICING PIPING**
## **<ins>GREPPING STORED RESULTS</ins>**
Redirecting the output and then grepping out the flag.

### SOLVE: 
***FLAG:*** pwn.college{oW_bOHXpQBsBRReBFId0QpNFyFM.QX4EDO0wSO2kjNzEzW}

First I redirected the output of /challenge/run to the file /tmp/data.txt.
Using the command /challenge/run > /tmp/data.txt.
Then I grepped the file /tmp/data.txt to find the flag.
Since every flag starts with pwn.college I used the command grep pwn.college /tmp/data.txt to obtain the flag.

```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn.college /tmp/data.txt
pwn.college{oW_bOHXpQBsBRReBFId0QpNFyFM.QX4EDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to redirect the output to a file and then find the flag in that file using the grep command.

### REFERENCES:
None.
