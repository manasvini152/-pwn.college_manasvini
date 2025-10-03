# **PONDERING PATHS**
## **<ins>IMPLICIT RELATIVE PATH</ins>**
We run this challenge from the /challenge directory and invoke the program from a relative path.
### SOLVE: 
***FLAG:*** pwn.college{MLDMKsTgOSUkXoSNFlw2ZvMsdBU.QXxUTN0wSO2kjNzEzW}

The /challenge/run command will not work here since it is not in the /challenge directory.
Hence we need to change the directory using the cd command to the directory /challenge using cd /challenge.
Once we are in the /challenge directory simply entering the command 'run' will not work here, it will give the message bash: run: command not found
Hence we need to explicitly use a relative path to invoke the run program.
We run the command ./run which is a relative path.
```
hacker@paths~implicit-relative-path:~$ /challenge/run
Incorrect...
You are not currently in the /challenge directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ run
bash: run: command not found
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{MLDMKsTgOSUkXoSNFlw2ZvMsdBU.QXxUTN0wSO2kjNzEzW}
```
### WHAT I LEARNED: 
I learnt how to invoke a program called run explixitly through a relative path, 
i also learnt why we cannot simply invoke run without a relative path.


### REFERENCES:
None.
