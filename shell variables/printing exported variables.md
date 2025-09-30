# **SHELL VARIABLES**
## **<ins>PRINTING EXPORTED VARIABLES</ins>** 
Instead of using the echo command to print exported variables we can use the env command.

### SOLVE: 
***FLAG:*** pwn.college{ca9HbZ1-4PHCYc3-fugygLzhZ6z.QX4UTN0wSO2kjNzEzW}

By using the command env, the output was printed which gave the flag under the FLAG variable.

```
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=379b958a3c71ffe92eeb9860920563bc94b475d615803d1d4c03ae80001c585b
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{ca9HbZ1-4PHCYc3-fugygLzhZ6z.QX4UTN0wSO2kjNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

### WHAT I LEARNED: 
I learnt about the env command which prints out every exported variable.

### REFERENCES:
None.

