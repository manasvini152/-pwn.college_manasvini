# **COMPREHENDING COMMANDS**
## **<ins>HIDDEN FILES</ins>**
We learn how to access hidden files through the ls command using the -a flag. The files are hidden when it starts with a '.'

### SOLVE: 
***FLAG:*** pwn.college{AqCK5GxtSZf5GsqjciLIN0p267P.QXwUDO0wSO2kjNzEzW}

At first when I used the ls command two non hidden files were shown, the question mentions that the fiag 
is in the / directory hence i changed the directory to / using the cd command.
Using the cd / and then accessing the hidden files using the command ls -a, we get a flag file.
Hence we open the file using the cat command and obtain the flag.

```
hacker@commands~hidden-files:~$ ls
delete_me  m
hacker@commands~hidden-files:~$ ls -a
.  ..  .bash_history  .config  delete_me  m
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-134161112910910  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-134161112910910
pwn.college{AqCK5GxtSZf5GsqjciLIN0p267P.QXwUDO0wSO2kjNzEzW}
```

### WHAT I LEARNED:  
I learnt how to access hidden files with the help of the command ls -a.
I also learnt how to hide a file using the . operator before naming the file.

### REFERENCES:
None.
