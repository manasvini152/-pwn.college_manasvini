# **CHAINING COMMANDS**
## **<ins>SCRIPTING WITH ARGUMENTS</ins>**
We create a shell script which accepts two arguments and outputs them in reverse order. 

### SOLVE: 
***FLAG:*** pwn.college{YBqZdrtMmBzaN5b41uJrrO_39uE.0VNzMDOxwSO2kjNzEzW}

We accept two arguments and print it in reverse order using $2 and $1 and by using the echo command.

```
hacker@chaining~scripting-with-arguments:~$ echo '#!/bin/bash' > /home/hacker/solve.sh
hacker@chaining~scripting-with-arguments:~$ echo 'echo "$2 $1"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-arguments:~$ bash /home/hacker/solve.sh hello world
world hello
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{YBqZdrtMmBzaN5b41uJrrO_39uE.0VNzMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
Learnt how to print the arguments in the order required.  

### REFERENCES:
None. 
