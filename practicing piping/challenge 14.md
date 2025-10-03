# **PRACTICING PIPING**
## **<ins>NAMED PIPES</ins>**
Usually temporary names are created for pipes but we can create our own names using mkfifo command.

### SOLVE: 
***FLAG:*** pwn.college{oFnfSxtxfB8x1QA37JjNGinF8Ui.01MzMDOxwSO2kjNzEzW}

Here we have to simultaneously work on two terminals due to the blocking feature of FIFO(first in first out).
Hence we read in one terminal and write in the other terminal.
In the first terminal I created a new fifo using the mkfifo command, I created the fifo /tmp/flag_fifo file.
Then I ran the cat command on /tmp/flag_fifo, initially there was no output because the file was empty. 
Now in the second terminal I ran the command /challenge/run > /tmp/flag_fifo which redirected /challenge/run
to the fifo at /tmp/flag_fifo.
Once this was done I went back to the first command and the flag was displayed since there was a file in 
/tmp/flag_fifo now.
By using two terminals we bypass the blocking feature of a FIFO.

**TERMINAL 1:**
```
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{oFnfSxtxfB8x1QA37JjNGinF8Ui.01MzMDOxwSO2kjNzEzW}
```

**TERMINAL 2:**
```
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
```

### WHAT I LEARNED:
I learnt about a FIFO and what it does. I also learnt about the advantages of using a FIFO.
And how to bypass the blocking feature of a FIFO.

### REFERENCES:
None.
