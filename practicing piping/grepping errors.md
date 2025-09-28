# **PRACTICING PIPING**
## **<ins>GREPPING ERRORS</ins>**
We can grep errors with the help of the command 2>& 1, and combine it with the pipe command to get the flag.

### SOLVE: 
***FLAG:*** pwn.college{44nHcsPM7PDQU_4tXzjmokCJFYu.QX1ATO0wSO2kjNzEzW}

By using the command /challenge/run 2>& 1 | grep pwn.college.
The errors are redirected from /challenge/run and then with the help of the grep command we grep the flag.
We use the pipe command to grep the flag. The 2>&1 command redirects the standard eroor to the standard output.

```
hacker@piping~grepping-errors:~$ /challenge/run 2>& 1 | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{44nHcsPM7PDQU_4tXzjmokCJFYu.QX1ATO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the command 2>& 1 and then how to grep the command using pipe operator.

### REFERENCES:
None.
