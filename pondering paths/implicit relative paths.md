# **PONDERING PATHS**
## **<ins>IMPLICIT RELATIVE PATHS, FROM /</ins>**
We need to run the /challenge/run command using a reltive path while having a current working directory of /.
### SOLVE: 
***FLAG:*** pwn.college{I2dzIe3l3NghlJ3WAGpJpdAYMm4.QX5QTN0wSO2kjNzEzW}

The current working directory cwd does not start with the root directory /. Hence we need to change the directory to the root directory.
without changing the directory /challenge/run will not work.
Hence we change the directory to /, using cd /
Now we use the challenge/run command since the cwd is already at / we do not need to enter /challenge/run. 
challenge/run is a relative path to the file.
thus we obtain the flag.
### WHAT I LEARNED: 
I learnt what a current working directory is, I also learnt about a relative path. and the difference between an absolute path and relative path.
### REFERENCES:
None.
