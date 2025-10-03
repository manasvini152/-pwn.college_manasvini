# **PONDERING PATHS**
## **<ins>POSITION YET ELSEWHERE</ins>**
We change directories by using the cd command and then run the current directory and the program under it.
### SOLVE: 
***FLAG:*** pwn.college{wqrNbA-YvynfgUeEdEkU4Z0ZXRx.QX4QTN0wSO2kjNzEzW}

I started with running the /challenge/run command which gave me a message that said I am not in the /home directory.
Then I had to use the cd command to change the directory to /home, after changing the directory I ran the /challenge/run command
Hence I obtained the flag.

```
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /home directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /home
hacker@paths~position-yet-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wqrNbA-YvynfgUeEdEkU4Z0ZXRx.QX4QTN0wSO2kjNzEzW}
```
### WHAT I LEARNED:
I learnt how to find out which directory a command is in and thus change directories and run the program.
### REFERENCES:
None.
