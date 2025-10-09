# **UNTANGLING USERS**
## **<ins>CRACKING PASSWORDS</ins>**
We have to crack the password in /challenge/shadow-leak and switch user to zardus  /challenge/run.

### SOLVE: 
***FLAG:*** pwn.college{Al1VKeJCIzf9UEZGYRquV5Es9xd.QX3UDN1wSO2kjNzEzW}

I first used john the ripper to crack the password. Once I got the password for zardus I used the su command and entered the password.
Doing this took me to the /home/hacker directory from where I ran the /challenge/run command and got the flag.

```
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:02 28% 1/3 0g/s 280.9p/s 280.9c/s 280.9C/s sudraz!..bzardus
Session aborted
hacker@users~cracking-passwords:~$ su zardus
Password:
su: Authentication failure
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:05 64% 1/3 0g/s 289.8p/s 289.8c/s 289.8C/s Zardus9999975..zardus99999F
0g 0:00:00:07 79% 1/3 0g/s 290.9p/s 290.9c/s 290.9C/s Zardus33..z99999000
0g 0:00:00:09 96% 1/3 0g/s 289.3p/s 289.3c/s 289.3C/s zardus999991963..zardus1939
0g 0:00:00:10 0% 2/3 0g/s 289.0p/s 289.0c/s 289.0C/s 123456
0g 0:00:00:11 0% 2/3 0g/s 289.2p/s 289.2c/s 289.2C/s purple..larry
0g 0:00:00:12 0% 2/3 0g/s 289.1p/s 289.1c/s 289.1C/s kelly..snickers
0g 0:00:00:13 0% 2/3 0g/s 289.2p/s 289.2c/s 289.2C/s francine..me
0g 0:00:00:14 0% 2/3 0g/s 289.3p/s 289.3c/s 289.3C/s Alexis..bigred
0g 0:00:00:15 0% 2/3 0g/s 289.6p/s 289.6c/s 289.6C/s grumpy..keeper
0g 0:00:00:16 0% 2/3 0g/s 289.7p/s 289.7c/s 289.7C/s rockie..surfing
0g 0:00:00:17 1% 2/3 0g/s 289.1p/s 289.1c/s 289.1C/s pretty..celtic
0g 0:00:00:18 1% 2/3 0g/s 289.0p/s 289.0c/s 289.0C/s chacha..jazmin
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04962g/s 288.9p/s 288.9c/s 288.9C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{Al1VKeJCIzf9UEZGYRquV5Es9xd.QX3UDN1wSO2kjNzEzW}
```

### WHAT I LEARNED:
I learnt about cracking passwords using the john command. I learnt about how and why passwords are not stored in /etc/shadow.

### REFERENCES:
None. 
