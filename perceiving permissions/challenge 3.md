# **PERCEIVING PERMISSIONS**
## **<ins>FUN WITH GROUPS NAMES</ins>**
We use the command id to check which groups we are a part of.

### SOLVE: 
***FLAG:*** pwn.college{YFo76N4SAIj_ljHiNUzg0DYeLA6.QXycjM1wSO2kjNzEzW}

By using the id command we get a list of the groups we are a part of. Hence we get the name of the group 
and now using the chgrp command and the group name and the file name. And then by catting out the file we get the flag.

```
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp25747) groups=1000(grp25747)
hacker@permissions~fun-with-groups-names:~$ chgrp grp25747 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{YFo76N4SAIj_ljHiNUzg0DYeLA6.QXycjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the id command to figure out the name of the group. 

### REFERENCES:
None. 
