# **PRACTICING PIPING**
## **<ins>REDIRECTING INPUT</ins>**
This challenge introduces us to the operator < to redirect the inputs.

### SOLVE: 
***FLAG:*** pwn.college{YV-SzA2xWpihHj6Ge_PQVzaRuBV.QXwcTN0wSO2kjNzEzW}

First I used the command echo COLLEGE > PWN to redirect the output COLLEGE to the file PWN.
Then I used the command /challenge/run < PWN to redirect the input.

```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{YV-SzA2xWpihHj6Ge_PQVzaRuBV.QXwcTN0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the redirecting input operator, <.

### REFERENCES:
None.
