# **PRACTICING PIPING**
## **<ins>PROCESS SUBSTITUTION FOR INPUT</ins>**
We use process substitution. Here we compare the output of two commands using the diff command.

### SOLVE: 
***FLAG:***  pwn.college{8YSzMKGAfAs6B7T37UbvPxrLlOm.0lNwMDOxwSO2kjNzEzW}

By using the command  diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag) we can find the difference between the output 
of the two commands /challenge/print_decoys and /challenge/print_decoys_and_flag.
The syntax for reading from a command is <(command), when we use this bash runs the command and stores the output in a temporary file.

```
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
66a67
> pwn.college{8YSzMKGAfAs6B7T37UbvPxrLlOm.0lNwMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about process substitution and how to read the output from a command using <(command).

### REFERENCES:
None.
