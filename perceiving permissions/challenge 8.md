# **PERCEIVING PERMISSIONS**
## **<ins>THE SUID BIT</ins>**
Suid means that regardless of what user runs the program the program will execute as the owner user.

### SOLVE: 
***FLAG:*** pwn.college{4OzIZWHTYpNvn_Cq4Fc1Xluf6Ex.QXzEjN0wSO2kjNzEzW}

By using the command chmod a+s /challenge/getroot we suid the program /challenge/getroot. After doing this when we run /challenge/getroot
it runs as a root and thus we have root access. Hence we can cat out the file since we have root access.
Using cat /flag we obtain the flag.

```
hacker@permissions~the-suid-bit:~$ chmod a+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{4OzIZWHTYpNvn_Cq4Fc1Xluf6Ex.QXzEjN0wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the suid command and how to gain root access.

### REFERENCES:
None. 
