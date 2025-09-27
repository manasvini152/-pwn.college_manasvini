# **DIGESTING DOCUMENTATION**
## **<ins>HELP FOR BUILTINS</ins>**
I learnt about the help command where the builtin command will read you the flag, if the right arguments are provided.

### SOLVE: 
***FLAG:*** pwn.college{I3SI3F1xU7Vt0w9Oa8ygg7T_1Xe.QX0ETO0wSO2kjNzEzW}

First I executed the help challenge command where I passed the challenge program to the help builtin.
Then I used the --secret VALUE command which prints the flag if the value is correct.
The value given is I3SI3F1x.
Hence by using the command challenge --secret I3SI3F1x we can obtain the flag.

```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "I3SI3F1x".
hacker@man~help-for-builtins:~$ challenge --secret I3SI3F1x
Correct! Here is your flag!
pwn.college{I3SI3F1xU7Vt0w9Oa8ygg7T_1Xe.QX0ETO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the help command. And when a command is built into the shell its called builtin.

### REFERENCES:
None.
