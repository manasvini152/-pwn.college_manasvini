# **DIGESTING DOCUMENTATION**
## **<ins>SEARCHING MANUALS</ins>**
I learnt how to search manuals with the help of the / operator. 

### SOLVE: 
***FLAG:*** pwn.college{0oX_EBITGiL7_1pehGbaJU4n2nA.QX1EDO0wSO2kjNzEzW}

Initially I used the man challenge command which displayed the manual page for challenge.
After entering the manual page I searched for the word flag with the help of the command, /flag.
By using the 'n' key to scroll, I found a line --uem  This argument will give you the flag!
Hence by clicking on q I quit the manual page.
Now by using the command /challenge/challenge  --uem I obtained the flag.

```
/challenge/challenge  --uem
hacker@man~searching-manuals:~$ /challenge/challenge  --uem
Initializing...
Correct usage! Your flag: pwn.college{0oX_EBITGiL7_1pehGbaJU4n2nA.QX1EDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to search for phrases in the manual, using the /.

### REFERENCES:
None.
