# **FILE GLOBBING**
## **<ins>MULTIPLE OPTIONS FOR TAB COMPLETION</ins>**
If there are multiple options for tab completion then by selecting tab the first time it will auto expand but when
you hit tab for the second time then it will print out all the options.

### SOLVE: 
***FLAG:*** pwn.college{wJ40sCPIXPXicmuY79OvxIkJMW5.0lN0EzNxwSO2kjNzEzW}

I entered  cat /challenge/files/p and hit the tab option which displayed cat /challenge/files/pwn then when I hit the tab key 
the second time a list of all options were displayed.
Then by running the command cat /challenge/files/pwncollege-flag the flag was displayed.

```
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter
pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{wJ40sCPIXPXicmuY79OvxIkJMW5.0lN0EzNxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about multiple options when using the tab completion and how to display all the options.

### REFERENCES:
None.
