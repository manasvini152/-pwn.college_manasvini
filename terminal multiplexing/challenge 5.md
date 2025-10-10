# **TERMINAL MULTIPLEXING**
## **<ins>DETACHING AND ATTACHING (TMUX)</ins>**

We learn about terminal multiplexer or tmux.

### SOLVE: 
***FLAG:*** pwn.college{g-sfYVuv6PeH3fX_3qlqTv_Y9Qu.0VO4IDOxwSO2kjNzEzW} 

We first run tmux and then dettach using ctrl+b d and then we run /challenge/run and reattach to tmux using tmux attach and obtain the flag.


```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
Flag sent! Now reattach to your tmux session with:
  tmux attach
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0scripts:~$
Sending flag to your tmux session...
You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux attach
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{g-sfYVuv6PeH3fX_3qlqTv_Y9Qu.0VO4IDOxwSO2kjNzEzW}
Congratulations, here is your flag: pwn.college{g-sfYVuv6PeH3fX_3qlqTv_Y9Qu.0VO4IDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about tmux and how to attach and detach from it.

### REFERENCES:
None. 
