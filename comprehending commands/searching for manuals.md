# **DIGESTING DOCUMENTATION**
## **<ins>SEARCHING FOR MANUALS</ins>**
We learn how to execute the man man command.

### SOLVE: 
***FLAG:*** pwn.college{gPaA03x6-_M0007egs2krYhx1Hh.QX2EDO0wSO2kjNzEzW}

I first ran the man man command and then ran the man -k flag command.
After running the man -k flag command, gaxegskrhx (1)       - print the flag! this command is displayed.
Then by running the command man gaxegskrhx. The description shows  --gaxegs NUM  print the flag if NUM is 036.
Hence by running the /challenge/challenge --gaxegs 036 command we obtain the flag.

```
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k flag
dpkg-buildflags (1)  - returns build flags to use during package build
Dpkg::BuildFlags (3perl) - query build flags
fegetexceptflag (3)  - floating-point rounding and exception handling
fesetexceptflag (3)  - floating-point rounding and exception handling
gaxegskrhx (1)       - print the flag!
i386 (8)             - change reported architecture in new program environment and/or set personality flags
ioctl_iflags (2)     - ioctl() operations for inode flags
linux32 (1)          - change reported architecture in new program environment and/or set personality flags
linux64 (1)          - change reported architecture in new program environment and/or set personality flags
pcap-config (1)      - write libpcap compiler and linker flags to standard output
security_compute_av_flags (3) - query the SELinux policy database in the kernel
security_compute_av_flags_raw (3) - query the SELinux policy database in the kernel
set_matchpathcon_flags (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure ...
set_matchpathcon_invalidcon (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and confi...
set_matchpathcon_printf (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure...
setarch (1)          - change reported architecture in new program environment and/or set personality flags
setarch (8)          - change reported architecture in new program environment and/or set personality flags
x86_64 (8)           - change reported architecture in new program environment and/or set personality flags
hacker@man~searching-for-manuals:~$ man gaxegskrhx
hacker@man~searching-for-manuals:~$ /challenge/challenge  --gaxegs 036
Correct usage! Your flag: pwn.college{gPaA03x6-_M0007egs2krYhx1Hh.QX2EDO0wSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the man man command and learnt more about the man command.

### REFERENCES:
None.
