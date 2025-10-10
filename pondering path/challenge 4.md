# **PONDERING PATH**
## **<ins>ADDING COMMANDS</ins>**

We make a shell script and and add its location to PATH.

### SOLVE: 
***FLAG:***  pwn.college{8hrcf9W_-7nZitRx9PHnjFJs8AD.QX2cjM1wSO2kjNzEzW}

I wrote a shell script and changed the permission for the user to execute it. 
I then exported the PATH variable for both the current directory and the path of the PATH variable.

```
hacker@path~adding-commands:~$ echo "cat /flag" > win
hacker@path~adding-commands:~$ chmod +x win
hacker@path~adding-commands:~$ export PATH="$(pwd):$PATH"
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{8hrcf9W_-7nZitRx9PHnjFJs8AD.QX2cjM1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt that we can add commands to PATH.

### REFERENCES:
None. 
