# **DIGESTING DOCUMENTATION**
## **<ins>HELPFUL PROGRAMS</ins>**
I learnt about the --help command, which can also be written as -h.

### SOLVE: 
***FLAG:*** pwn.college{UdmvbJOHnJAjoZ58JP9nWyfK9T8.QX3IDO0wSO2kjNzEzW}

First I executed the commmand /challenge/challenge --help which gave me a list of optional arguments.
Later on I executed the  /challenge/challenge -p command and got the secret value, the -p command prints the value that causes the -g 
option to give the flag. Then I executed the -g command along with the secret value to get the flag. The -g command is the give flag 
command which gives us the flag when the secret key is entered along with the command.
The command was /challenge/challenge -g 589.

```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 589
hacker@man~helpful-programs:~$ /challenge/challenge -g 589
Correct usage! Your flag: pwn.college{UdmvbJOHnJAjoZ58JP9nWyfK9T8.QX3IDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the --help command, the -p command and the -g command.

### REFERENCES:
None.
