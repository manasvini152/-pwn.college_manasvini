# **PONDERING PATHS**
## **<ins>PROGRAM AND ABSOLUTE PATHS</ins>**
We access the root directory and then the challenge directory and then the program.
### SOLVE: 
***FLAG:*** pwn.college{cuz0lf-p9i_caS4on2v8PsRp_P3.QX1QTN0wSO2kjNzEzW}

We start with a / to access the root directory and then we access the challenge directory /challenge which is the path to the challenge directory,
and then we access the program named run, /challenge/run
we execute it by invoking the absolute path, and hence we execute the run file which is in the challenge directory which is in the root directory. 
```
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{cuz0lf-p9i_caS4on2v8PsRp_P3.QX1QTN0wSO2kjNzEzW}
```
### WHAT I LEARNED:
I learnt how to invoke a directory in the root directory and execute a program in the existing directory.
### REFERENCES:
None.

