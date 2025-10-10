# **CHAINING COMMANDS**
## **<ins>UNDERSTANDING SHEBANGS</ins>**
The shell script we create at /home/hacker/solve.sh should have a proper shebang and outputs "hack the planet".

### SOLVE: 
***FLAG:*** pwn.college{QBfdevxz3akZiOayncG5Hew-fCK.0VOzMDOxwSO2kjNzEzW}

I created a shell script with a shebang. I then gave permissions to the user using chmod.
Then by running the /challenge/run we get the flag. 

```
hacker@chaining~understanding-shebangs:~$ echo '#!/bin/bash' > /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ echo 'echo "hack the planet"' >> /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ chmod u+xwr /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{QBfdevxz3akZiOayncG5Hew-fCK.0VOzMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about shebangs and if the program file starts with the characters #! it is a shebang.

### REFERENCES:
None. 
