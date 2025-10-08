# **UNTANGLING USERS**
## **<ins>BECOMING ROOT WITH SU</ins>**
We become the root with su by entering the password.

### SOLVE: 
***FLAG:*** pwn.college{EnOrBVSnOfRM24RnaaZI_JnfQN0.QX1UDN1wSO2kjNzEzW}

We run the su command and enter the password as hack-the-planet. After the correct passowrd is entered. The root was made.
Then on using the ls command I saw the list of directories and then by catting out the file not-the-flag we obtain the flag.

```
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# ls
COLLEGE  FD_CLOEXEC  PWN  delete_me  instructions  m  myflag  not-the-flag  pwn  the-flag
root@users~becoming-root-with-su:/home/hacker# cat not-the-flag
pwn.college{EnOrBVSnOfRM24RnaaZI_JnfQN0.QX1UDN1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the su command and how to become the root.

### REFERENCES:
None. 
