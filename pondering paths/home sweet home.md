# **PONDERING PATHS**
## **<ins>HOME SWEET HOME</ins>**
We learn about home directory, since our username is hacker /home/hacker.
### SOLVE: 
***FLAG:*** pwn.college{MivIgiyKQuar6LgDQI0nX1jxtYM.QXzMDO0wSO2kjNzEzW}

The home directory is where we store most of our files. The ~ is a shorthand for /home/hacker 
when we invoke /challenge/run ~/m which is an absolue path and m is a file name given by the user.
/challenge/run ~/m expands to /challenge/run /home/hacker/m.
where home is nothing but a direcroty, when this is invoked we get the flag.
```
hacker@paths~home-sweet-home:~$ /challenge/run ~/m
Writing the file to /home/hacker/m!
... and reading it back to you:
pwn.college{MivIgiyKQuar6LgDQI0nX1jxtYM.QXzMDO0wSO2kjNzEzW}
```
### WHAT I LEARNED: 
I learnt what a ~ does and what the expansion is. I also learnt about arguments
Where an argument is an absolute path and and it must be inside the home directory, and it should be three characters or less.

### REFERENCES:
None.
