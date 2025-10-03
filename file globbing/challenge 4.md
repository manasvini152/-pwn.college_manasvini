# **FILE GLOBBING**
## **<ins>MATCHING PATHS WITH []</ins>**
This challenges shows how to glob starting from home directory with a path.

### SOLVE: 
***FLAG:*** pwn.college{IPVebsaci-k-krulw6LDlv9Erv2.QX0IDO0wSO2kjNzEzW}

First we need the directory to be in the default /home/hacker directory.
Then we run the file_bash command under the /challenge/files directory under /challenge/run.
Hence we obtain the flag.

```
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{IPVebsaci-k-krulw6LDlv9Erv2.QX0IDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about globbing through path basis.

### REFERENCES:
None.
