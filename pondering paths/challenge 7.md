# **PONDERING PATHS**
## **<ins>EXPLICIT RELATIVE PATHS, FROM /</ins>**
We learn about explicit relative paths and the use of . and .. operator. 
### SOLVE: 
***FLAG:*** pwn.college{EwOu_Jge2JR-hPAoNsDfQM7964U.QXwUTN0wSO2kjNzEzW}

First I switched to the / directory by using the change directory [cd] command.

the challenge/run command does not work here since it is not implicit.

Thus this challenge must be called with a relative path that explicitly starts with a '.'

hence when we enter the ./challenge/run command we obtain the flag.

therefore ./challenge/run is a relative path because of the use of '.' and belongs to the directory /.

If the cwd is / the relative paths are equivalent to the absolute paths. 

```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ challenge/run
Incorrect...
This challenge must be called with a relative path that explicitly starts with a `.`!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{EwOu_Jge2JR-hPAoNsDfQM7964U.QXwUTN0wSO2kjNzEzW}
```
### WHAT I LEARNED: 
I learnt about relative paths and the use of . operator. I learnt how to explicitly call a challenge with the help of relative path.
Also learnt about identical absolute and relative paths. 

### REFERENCES:
None.
