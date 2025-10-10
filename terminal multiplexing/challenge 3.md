# **TERMINAL MULTIPLEXING**
## **<ins>FINDING SESSIONS</ins>**
We use the screen -ls command. To list out the screen contents.

### SOLVE: 
***FLAG:*** pwn.college{0MgnnzwKL6AcWOHVFr3MveCAXja.01N4IDOxwSO2kjNzEzW}

We use the screen -ls command and then screen -r along with session name which gives us the flag under the second session.

```
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        165.pts-1.terminal-multiplexing~launching-screen        (Remote or dead)
        154.pts-1.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        144.session_31772c102885257b    (Attached)
        147.session_59d4f7227845b6da    (Detached)
        150.session_ee5b859f4c61de91    (Detached)
5 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_31772c102885257b
[detached from 144.session_31772c102885257b]minal-multiplexing~detaching-and-attaching
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_59d4f7227845b6da
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{0MgnnzwKL6AcWOHVFr3MveCAXja.01N4IDOxwSO2kjNzEzW}
pwn.college{0MgnnzwKL6AcWOHVFr3MveCAXja.01N4IDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about how to see the sessions and the contents of the sessions.

### REFERENCES:
None. 

