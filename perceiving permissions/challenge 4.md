# **PERCEIVING PERMISSIONS**
## **<ins>CHANGING PERMISSIONS</ins>**
The commands u,g and o stands for users, groups and other users respectively. 
The commands r,w and x stands for read, write and execute respectively.

### SOLVE: 
***FLAG:*** pwn.college{0UiDhdiSUwWDAMPYhln0H1_xC3u.QXzcjM1wSO2kjNzEzW}

By using the command chmod the mode is changed, and the command a+rwx changes all users, groups and other users permissions to 
read, write and execute. Then by catting out the file we obtain the flag.

```
hacker@permissions~changing-permissions:~$ chmod a+rwx /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{0UiDhdiSUwWDAMPYhln0H1_xC3u.QXzcjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the command a+rwx and what it stands for.

### REFERENCES:
None. 
