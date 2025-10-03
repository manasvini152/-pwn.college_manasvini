# **PONDERING PATHS**
## **<ins>POSITION THY SELF</ins>**
We change directories by using the cd command and then run the current directory and the program under it.
### SOLVE: 
***FLAG:*** pwn.college{Io3eX_Rk-K9pjFCcXz50x4RUP0L.QX2QTN0wSO2kjNzEzW}

I started with running the /challenge/run command similar to the previous challenge, I got a message saying that it is incorrect and that I have to change directories.
Below the incorrect command I received a directory /usr/share/zoneinfo/posix/Asia which I had to change to.
Using the change directory [cd] command, I entered cd /usr/share/zoneinfo/posix/Asia which changed the directory.
After I was in the new directory I ran the /challenge/run command which is an absolute path and was invoked from the directory /usr/share/zoneinfo/posix/Asia.
Hence I received the flag.
```
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/zoneinfo/posix/Asia directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd  /usr/share/zoneinfo/posix/Asia
hacker@paths~position-thy-self:/usr/share/zoneinfo/posix/Asia$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Io3eX_Rk-K9pjFCcXz50x4RUP0L.QX2QTN0wSO2kjNzEzW}
```
### WHAT I LEARNED:
I learnt how to change directories and run programs after changing the directory.
### REFERENCES:
None.
