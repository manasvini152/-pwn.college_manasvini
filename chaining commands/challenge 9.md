# **CHAINING COMMANDS**
## **<ins>SCRIPTING WITH CONDITIONALS</ins>**
We use the if command and abide by all the rules.

### SOLVE: 
***FLAG:***  pwn.college{wz62AG3VOCMXHO7F_v6B0rPqHFy.0lNzMDOxwSO2kjNzEzW}

I entered the code according to the conditions of the if statements. That is if pwn was entered the output was supposed to be college 
and the if statement must end with fi. And there must spaces before and after [ and ] and after if.

```
hacker@chaining~scripting-with-conditionals:~$ echo '#!/bin/bash' > /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ echo 'if [ "$1" = "pwn" ]' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$  echo 'then' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ echo '    echo "college"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ echo 'fi' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ chmod u+x /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{wz62AG3VOCMXHO7F_v6B0rPqHFy.0lNzMDOxwSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about the if statments and all the conditions applicable.

### REFERENCES:
None. 

