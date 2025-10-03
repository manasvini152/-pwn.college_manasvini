# **COMPREHENDING COMMANDS**
## **<ins>MOVING FILES</ins>**
We learn about the mv command which moves files around, from one place to another.

### SOLVE: 
***FLAG:*** pwn.college{k1hXmhRXDtgJGDT5k-v-NOoU1s0.0VOxEzNxwSO2kjNzEzW}

First I moved the /flag file to /tmp/hack-the-planet using the mv command.
The command is mv /flag /tmp/hack-the-plane.
Once it is moved we execute the /challenge/check command to obtain the flag.

```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{k1hXmhRXDtgJGDT5k-v-NOoU1s0.0VOxEzNxwSO2kjNzEzW}

```
### WHAT I LEARNED:  
I learnt how to move files around using the mv command, it moves the files as well as the contents in the file.

### REFERENCES:
None.
