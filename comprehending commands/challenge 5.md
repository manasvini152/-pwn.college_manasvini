# **COMPREHENDING COMMANDS**
## **<ins>COMPARING FILES</ins>**
We learn about the diff command which gives us the difference between two files. It compares each file line by line and gives the difference.
### SOLVE: 
***FLAG:*** pwn.college{EtoV2orAyucA2-H38E3mLhgealP.01MwMDOxwSO2kjNzEzW}

The two files given to us is /challenge/decoys_only.txt and /challenge/decoys_and_real.txt where the second files contains all the flags in 
the first file along with one additional flag which is real.
Hence by finding the difference between these two files we can obtain the real flag.
By using the command diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt we can obtain the flag.
We get the output of 47a48 which means after line 47 of file 1, add line 48 of file 2.

```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
47a48
> pwn.college{EtoV2orAyucA2-H38E3mLhgealP.01MwMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:  
I learnt how to find the difference between two similar files. And how to use the diff command and what outputs like 2c2 and 1a2 means.

### REFERENCES:
None.
