# **CHAINING COMMANDS**
## **<ins>SCIRPTING WITH MULTIPLE CONDITIONS</ins>**
We use the commands similar to else if which is elif.

### SOLVE: 
***FLAG:*** pwn.college{onOeslqqtVHrId4qwhRhlHWsqMv.0FOzMDOxwSO2kjNzEzW}

I used the same logic as if and else command and combined them using elif command.

```
hacker@chaining~scripting-with-multiple-conditions:~$ echo '#!/bin/bash' > /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'if [ "$1" == "hack" ]; then' >> /home/hacker/solve.sh ; echo '    echo "the planet"' >> /home/hacker/solve.sh ; echo 'elif [ "$1" == "pwn" ]; then' >> /home/hacker/solve.sh ; echo '    echo "college"' >> /home/hacker/solve.sh ; echo 'elif [ "$1" == "learn" ]; then' >> /home/hacker/solve.sh ;  echo '    echo "linux"' >> /home/hacker/solve.sh ;  echo 'else' >> /home/hacker/solve.sh ;  echo '    echo "unknown"' >> /home/hacker/solve.sh ; echo 'fi' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ chmod u+wxr /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{onOeslqqtVHrId4qwhRhlHWsqMv.0FOzMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt the syntax of elif and how we can use it to script multiple conditionals.

### REFERENCES:
None. 
