# **PONDERING PATHS**
## **<ins>THE ROOT</ins>**
Here the filesystem starts at /. Which is the root directory. Inside the root directory a program called pwn is added.
### SOLVE: 
***FLAG:*** pwn.college{YDziWS8ZtaD3-XIAVD5zjkqOsNc.QX4cTO0wSO2kjNzEzW}

When we start with / the root directory is invoked. Under the / there is a program called pwn which has to be invoked in order to obtain the flag. When we use the / it is known as an absolute path.
It is an absolute path when it starts from the root directory. Here we invoke the program pwn using an absolute path. By entering /pwn the flag is obtained.
```
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{YDziWS8ZtaD3-XIAVD5zjkqOsNc.QX4cTO0wSO2kjNzEzW}
```
### WHAT I LEARNED:
I learnt how to invoke a program using an absolute path and I learnt about the root directory. When we use the slash the path starts from the root.
### REFERENCES:
None.
