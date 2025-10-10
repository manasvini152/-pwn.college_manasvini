# **TERMINAL MULTIPLEXING**
## **<ins>SWITCHING WINDOWS (TMUX)</ins>**

We must switch windows to get the flag.

### SOLVE: 
***FLAG:***  pwn.college{ckzj149WMT3iOXab8NSFI7Qm33q.0FM5IDOxwSO2kjNzEzW}

I connected using tmux attach and switched to the welcome window and then switched to window 0 using ctrl+b and 0 and got the flag.

```
hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux attach
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Welcome to the tmux window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-B 0 to switch to window 0!
> MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag:  pwn.college{ckzj149WMT3iOXab8NSFI7Qm33q.0FM5IDOxwSO2kjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag:  pwn.college{ckzj149WMT3iOXab8NSFI7Qm33q.0FM5IDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to switch tmux windows.

### REFERENCES:
None. 
