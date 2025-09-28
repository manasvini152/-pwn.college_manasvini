# **PRACTICING PIPING**
## **<ins>FILTERING WITH GREP -V</ins>**
The grep -v command filters out lines that does not match the pattern. It is the invert match.

### SOLVE: 
***FLAG:*** pwn.college{8zuvZeB-fthboZNnd-kaQ3FPB4l.0FOxEzNxwSO2kjNzEzW}

As the challenge mentions that the flags that are not real contain the word DECOY.
Hence by using the invert match we can find the real flag.
The flag is present in /challenge/run and by using the grep -v DECOY command it prints the flag that does not have 
the word DECOY in it. Hence we obtain the real flag.

```
hacker@piping~filtering-with-grep-v:~$  /challenge/run | grep -v DECOY
pwn.college{8zuvZeB-fthboZNnd-kaQ3FPB4l.0FOxEzNxwSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the invert match. And how to filter out lines that match the word provided.

### REFERENCES:
None.

