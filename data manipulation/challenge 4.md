# **DATA MANIPULATION**
## **<ins>EXTRACTING THE FIRST LINES WITH HEAD</ins>**
The head command prints the first 10 lines of the output.

### SOLVE: 
***FLAG:*** pwn.college{sy93fuRYbpXepFJdQLGhX86DjuA.0lNxEzNxwSO2kjNzEzW}

The challenge mentions that /challenge/pwn outputs a bunch of data and that we have to pipe it through head to get the first 7 lines,
and then pipe onwards to /challenge/college.
Hence by using the command /challenge/pwn | head -n 7 | /challenge/college we get the flag.
The -n command helps us to control the number of lines printed in the output.

```
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{sy93fuRYbpXepFJdQLGhX86DjuA.0lNxEzNxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the head command and how to specify the number of lines printed using the head and -n command.

### REFERENCES:
None. 
