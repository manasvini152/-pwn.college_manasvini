# **UNTANGLING USERS**
## **<ins>USING SUDO</ins>**
We use the sudo command to access and obtain the flag.

### SOLVE: 
***FLAG:*** pwn.college{0zDwTe0QgtJnVaXrTlChu5vgGXB.QX4UDN1wSO2kjNzEzW}

Using the ls command I listed out the contents of the directory, the flag was in the file not-the-flag.
Hence with the help of the cat and sudo command I obtained the flag.

```
hacker@users~using-sudo:~$ ls
COLLEGE  FD_CLOEXEC  PWN  delete_me  instructions  m  myflag  not-the-flag  pwn  the-flag
hacker@users~using-sudo:~$ sudo cat not-the-flag
pwn.college{0zDwTe0QgtJnVaXrTlChu5vgGXB.QX4UDN1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the sudo command and that it runs commands as the root itself instead of switching to the root.

### REFERENCES:
None. 
