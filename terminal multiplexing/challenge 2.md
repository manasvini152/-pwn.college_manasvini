# **TERMINAL MULTIPLEXING**
## **<ins>DETACHING AND ATTACHING</ins>**

We learn how to detach and attach to the screen.

### SOLVE: 
***FLAG:***  pwn.college{k8lf-ko2qFiZo4MUfk9F4qJ-jdA.0lN4IDOxwSO2kjNzEzW}

We detach using Ctrl+a and followed by d and run /challenge/run and then reattach using screen -r.


```
hacker@terminal-multiplexing~launching-screen:~$ screen
[detached from 154.pts-1.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 154.pts-1.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session... hacker@dojo.pwn.college
Connected!
Flag sent! Now reattach to your screen session with:nge/run
#!/opt/pwn.college/bash
  screen -r
read GUESS
You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen -r
hacker@terminal-multiplexing~detaching-and-attaching:~$ echo Yes! Flag is: pwn.college{k8lf-ko2qFiZo4MUfk9F4qJ-jdA.0lN4IDOxwSO2kjNzEzW}
Yes! Flag is: pwn.college{k8lf-ko2qFiZo4MUfk9F4qJ-jdA.0lN4IDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt how to detach and re attach to a screen.

### REFERENCES:
None. 
