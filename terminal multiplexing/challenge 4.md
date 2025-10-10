# **TERMINAL MULTIPLEXING**
## **<ins>SWITCHING WINDOWS</ins>**

Two windows are created and we have to switch from one window to the other.

### SOLVE: 
***FLAG:*** pwn.college{0AZzEO0BiqI43RBcMFJYPrXLCsX.0FO4IDOxwSO2kjNzEzW}

We run screen -r and the default window is 1 here and we switch to window 0 using Ctrl+a 0 and get the flag.


```
hacker@terminal-multiplexing~switching-windows:~$ screen -r
 cat <<MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Welcome to the window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-A 0 to switch to window 0!
> MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!

hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{0AZzEO0BiqI43RBcMFJYPrXLCsX.0FO4IDOxwSO2kjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{0AZzEO0BiqI43RBcMFJYPrXLCsX.0FO4IDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to switch from one window to the other.

### REFERENCES:
None. 
