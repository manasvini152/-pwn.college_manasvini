# **PRACTICING PIPING**
## **<ins>SPLIT-PIPING STDERR AND STDOUT</ins>**
We use the commands >(), 2> and | to obtain the flag.

### SOLVE: 
***FLAG:*** pwn.college{kL5onebgKT9Lt1EV4rebxgolcCO.QXxQDM2wSO2kjNzEzW}

Using the command  /challenge/hack > >(/challenge/planet) 2> >(/challenge/the).
We run the output of /challenge/hack through /challenge/planet and the error through /challenge/the.
Hence the we redirect /challenge/hack's stderr to /challenge/the using the command 2>
and we redirect /challenge/hack's stdout to /challenge/planet using the command >().

```
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet) 2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{kL5onebgKT9Lt1EV4rebxgolcCO.QXxQDM2wSO2kjNzEzW}

```

### WHAT I LEARNED: 
I learnt how to combine the different commands in piping. I also implemented the other way of piping data using > > command.

### REFERENCES:
None.
