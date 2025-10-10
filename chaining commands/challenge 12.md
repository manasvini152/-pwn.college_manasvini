# **CHAINING COMMANDS**
## **<ins>READING SHELL SCRIPTS</ins>**
We read the shell script by running /challenge/run and enter a secret password to get the flag.

### SOLVE: 
***FLAG:*** pwn.college{Q4Fp12Z5kClXx0q5nn9P3CiVknA.0lMwgDOxwSO2kjNzEzW}

Using the cat /challenge/run command I then ran /challenge/run command and by entering the secret key which was 'hack the PLANET'.
We obtain the flag.

```
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{Q4Fp12Z5kClXx0q5nn9P3CiVknA.0lMwgDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt cat can be used to read shell scripts.

### REFERENCES:
None. 
