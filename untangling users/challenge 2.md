# **UNTANGLING USERS**
## **<ins>OTHER USERS WITH SU</ins>**
With the hlep of the su command we can give a username as an argument and switch to that user instead. 

### SOLVE: 
***FLAG:*** pwn.college{QP6X2ggWRWLXIBQSLm-y6YsCZWV.QX2UDN1wSO2kjNzEzW}

We use the su command to switch to the zardus user. And the password being dont-hack-me as mentioned in the challenge description. 
Later on by running the /challenge/run command we obtain the flag.

```
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{QP6X2ggWRWLXIBQSLm-y6YsCZWV.QX2UDN1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to switch to another user using the su command.

### REFERENCES:
None. 
