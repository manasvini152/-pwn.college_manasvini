# **FILE GLOBBING**
## **<ins>TAB COMPLETION ON COMMANDS</ins>**
Tab completion can also be used on commands and need not be restricted to files only.

### SOLVE: 
***FLAG:*** pwn.college{wCcHF_GWgi5_3PSpw_mJYHkiox5.0VN0EzNxwSO2kjNzEzW}

I typed the command pwncollege and hit the tab key which displayed pwncollege-6061, upon pressing tab key again
I got all the options. But after invoking the command pwncollege-6061 the flag was displayed.

```
hacker@globbing~tab-completion-on-commands:~$ pwncollege-6061
.bash_history  .config/       .lesshst       delete_me      m
hacker@globbing~tab-completion-on-commands:~$ pwncollege-6061
Correct! Here is your flag:
pwn.college{wCcHF_GWgi5_3PSpw_mJYHkiox5.0VN0EzNxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt that the tab completion key is not only restricted to files but can also be used for commands.

### REFERENCES:
None.
