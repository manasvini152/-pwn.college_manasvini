# **COMPREHENDING COMMANDS**
## **<ins>AN EPIC FILE SYSTEM QUEST</ins>**
Here with the help of cd, ls and cat commends we attemp to find the flag.

### SOLVE: 
***FLAG:***  pwn.college{woZprfWl7uh4cP3We0JZXcZYibQ.QX5IDO0wSO2kjNzEzW}

First I changed the directory to / using the cd command.
After changing the directory I listed out the directory using the ls -a command.
After listing it out there was a file named INSIGHT, which I catted out using the cat 
INSIGHT command.
The next clue was in /opt/linux/linux-5.4/arch/openrisc/include/uapi/asm, hence I 
used the cd command to change directory.
Using cd /opt/linux/linux-5.4/arch/openrisc/include/uapi/asm
By using the ls command again I file named BRIEF was displayed.
By catting out the file using cat BRIEF. 
The next clue  /usr/lib/R was displayed. It is a trapped file and hence we cannot
use the cd command.
I used the ls  /usr/lib/R command which gave a file named SPOILER-TRAPPED.
Then I used the command cat /usr/lib/R/SPOILER-TRAPPED which gave me the next clue.
/usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace.

Hence by using the cd /usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace
and using the ls -a command a file named NUGGET was displayed.
By catting out NUGGET we get the next clue that is
/usr/share/locale/zh_CN/LC_MESSAGES.

By using cd /usr/share/locale/zh_CN/LC_MESSAGES and then using ls -a we get a file
named .CLUE. By catting the file we get /usr/share/doc/mysql-common/frozen-mode.

Again by using cd /usr/share/doc/mysql-common/frozen-mode and then ls -a, we get a 
file named EVIDENCE. By catting out EVIDENCE, we get 
 /opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm.

 I used cd  /opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm which gave me .MESSAGE
 then I used cat .MESSAGE which displayed  /opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for.

 Using cd  /opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for, and then ls -a 
 we get a file named HINT. Using cat HINT  we get /usr/lib/python3/dist-packages/scipy/constants

 Using cd /usr/lib/python3/dist-packages/scipy/constants then ls -a, we get .DISPATCH
 cat .DISPATCH gives us the flag.

 ```
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
..  INSIGHT     boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~an-epic-filesystem-quest:/$ cat INSIGHT
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/openrisc/include/uapi/asm
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.4/arch/openrisc/include/uapi/asm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/openrisc/include/uapi/asm$ ls
BRIEF  Kbuild  byteorder.h  elf.h  param.h  ptrace.h  sigcontext.h  unistd.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/openrisc/include/uapi/asm$ cat BRIEF
Great sleuthing!
The next clue is in: /usr/lib/R

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
ch/openrisc/include/uapi/asm$ ls /usr/lib/R
COPYING          SVN-REVISION  etc  library  site-library
SPOILER-TRAPPED  bin           lib  modules
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/openrisc/include/uapi/asm$ cat /usr/lib/R/SPOILER-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/openrisc/include/uapi/asm$ cd /usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace$ ls -a
.  ..  NUGGET  Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace$ cat NUGGET
Lucky listing!
The next clue is in: /usr/share/locale/zh_CN/LC_MESSAGES

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/STIX-Web/Monospace$ cd /usr/share/locale/zh_CN/LC_MESSAGES
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/zh_CN/LC_MESSAGES$ ls -a
.        fish.mo        iso_3166.mo    iso_639.mo
..       iso_15924.mo   iso_3166_2.mo  iso_639_3.mo
.CLUE    iso_3166-1.mo  iso_4217.mo    libapt-pkg6.0.mo
apt.mo   iso_3166-2.mo  iso_639-2.mo   sphinx.mo
dpkg.mo  iso_3166-3.mo  iso_639-3.mo
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/zh_CN/LC_MESSAGES$ cat .CLUE
Tubular find!
The next clue is in: /usr/share/doc/mysql-common/frozen-mode
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/zh_CN/LC_MESSAGES$ cd /usr/share/doc/mysql-common/frozen-mode
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/mysql-common/frozen-mode$ ls -a
.  ..  EVIDENCE  README  downgrade
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/mysql-common/frozen-mode$  cat EVIDENCE
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/mysql-common/frozen-mode$ cd /opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm$ ls -a
.   .MESSAGE  aon_defs.h  pm-mips.c  s2-arm.S   s3-mips.S
..  Makefile  pm-arm.c    pm.h       s2-mips.S
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm$ cat .MESSAGE
Yahaha, you found me!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/soc/bcm/brcmstb/pm$ cd /opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for$ ls -a
.  ..  HINT  buggy
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for$ cat HINT
Yahaha, you found me!
The next clue is in: /usr/lib/python3/dist-packages/scipy/constants

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/udhcpc/slack/for$ cd /usr/lib/python3/dist-packages/scipy/constants
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/scipy/constants$ ls -a
.   .DISPATCH    __pycache__  constants.py
..  __init__.py  codata.py    tests
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/scipy/constants$ cat .DISPATCH
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{woZprfWl7uh4cP3We0JZXcZYibQ.QX5IDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt how to find the flag using ls -a, cd and cat commands.

### REFERENCES:
None.
