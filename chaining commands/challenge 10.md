# **CHAINING COMMANDS**
## **<ins>SCRIPTING WITH DEFAULT CASES</ins>**
We use the if commands along with the else command. 

### SOLVE: 
***FLAG:*** pwn.college{ImxxAr8KeEbVFA6-sgQKrsaDp9T.01NzMDOxwSO2kjNzEzW}

The challenge is similar to the previous challenge except the else condition is added.

```
hacker@chaining~scripting-with-default-cases:~$ echo '#!/bin/bash' > /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo 'if [ "$1" = "pwn" ]' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo 'then' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '    echo "college"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo 'else' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '    echo "nope"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo 'fi' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ chmod u+x /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{ImxxAr8KeEbVFA6-sgQKrsaDp9T.01NzMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I leanrt about the else command and its syntax.

### REFERENCES:
None. 
