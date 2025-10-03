# **DATA MANIPULATION**
## **<ins>SORTING DATA</ins>**
We can sort the data in a file with the help of the sort command.

### SOLVE: 
***FLAG:*** pwn.college{s5M-pVef0RPJil28hCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}

With the help of the sort command the data can be sorted in the alphabetical order. 
By using arguments like -r ( reverse order ), -n ( numeric sort ), -u (removes duplicates) and -R (random order) we can modify the sort.
The challenge tells us that if sorted in alphabetical order the last flag is the real flag.
Hence by using the command  sort /challenge/flags.txt we obtain the flag.

```
hacker@data~sorting-data:~$ sort /challenge/flags.txt
ovm.bollegd{s5L-pVde0RPJil28hCL5RIO6_uG.0EM0MDNxwSO2kjNzDzW}
ovn.bokldge{r5M-pUdf0ROJil18hBL5QIO6_uG.0FM0MDOwwRO2jiMzDyW}
ovn.bolldge{s5M-pVef0QOJil28gCK5RIN6_tH.0FL0MDOxwRN2kjNzEzW}
ovn.cokkdgd{r5M-pVef0RPJil28gBL5RIN6_uH.0FM0LCNxvSN1jjMzDyW}
owm.cokldge{s5M-pVef0RPJhl27gCL5RIO6_tH.0FM0LDNwwSN2jiNzEyW}
owm.coklege{s5M-pVee0RPJil28hBL5RIO6_uH.0EM0MDOxwSO1jjNyEzW}
owm.colldge{r4L-pVef0ROIik28hCL5RIO6_uH.0FM0MCOwwSO1jiNzDzV}
owm.collefd{s5L-pVdf0RPJil18hCL5RIN6_uH.0FM0MDOxwRO2kjNzEzW}
owm.college{s5M-pVef0RPIil18hBL5RIO5_uH.0FL0MDOxwSO2kjNzEzV}
own.bnlldgd{r5M-pVee0QOIil17hCK5RHN5_uG.0FM0MDOxvSO2kjNzEyW}
own.bollege{s5L-pVef0RPJil28gCL5QIO6_uH.0EM0LDOxwSN2kjNyEzW}
own.cnkkdfe{s4M-pVee0QPJik27hBL5RHN5_uG.0FM0MDOxvSO2jjNyDzW}
own.cnlkdge{r5L-oVee0ROJil27hCL5RHO6_uH.0FM0MCOxwRO2kjNzEzW}
own.cnlkegd{r5L-pVef0RPIhk17hBL5QHO6_tH.0FM0MDOxwSO1kiNzDzW}
own.cnlkege{r5M-pVef0RPJil28gCL5RIO6_uG.0FM0MDOxwSO2kjNyEzW}
own.cnlldgd{s5M-pVdf0RPIhl27gCK5RIO6_uH.0EM0MCNxvSO1kjNzEyW}
own.colldgd{r4L-oVdf0RPIhl28hBL5RIO6_uH.0FL0LDOxwSO2kiNyDyW}
own.colldge{r5L-oVef0RPJil27hCK5RHN6_uH.0FM0MDOxvRO2kiNyDzV}
own.colldge{s5M-pUde0QOJil27hBK5QIN5_uH.0FL0MDNwvRN1kjNzDyW}
own.collefe{s5L-pVef0RPJil28hCK5QIO6_uH.0EM0LCNxwSO1kjNzEzW}
own.collefe{s5M-pUef0QOJil28hCL5QHO6_tG.0FM0MDOxwSO2kjNyEzW}
own.collefe{s5M-pVef0RPJil28hCL5RIO6_uH.0FM0MCOxwSO2kiMzEzW}
own.college{r4M-pVef0RPJil28hCK5RIO6_uH.0FM0MDOxwSO2kjNyEzW}
own.college{s5M-pUdf0RPJhk28hBL5RIN5_tH.0FM0MDOxwSN1kiNyEyV}
pvm.bnkldfd{r5L-pVee0QPIhk17hCL5RIO6_uH.0EM0MCOxwSO2kjMyDzW}
pvm.bolldge{s5L-pVef0ROIik18hBL5RIO6_uH.0EM0MCOwvSN1kjNzEyW}
pvm.cnlldfe{r4L-oUdf0QPJil27hCK4QHO6_tG.0FM0LDOxwSO2kjMzEzW}
pvm.cokkdge{s4M-pUee0QOJil28hBL5RIO6_uG.0FL0MDOwwSO2kiNzEzV}
pvm.college{s5M-pVdf0RPIil18hCL5QIO5_uH.0EM0MDOxwRN1kiNzDzV}
pvn.bokkegd{s5M-oVef0RPJil28hCL5QHO6_uH.0FM0MDOwvRO2kjNzEzW}
pvn.boklefe{s4M-pVee0RPJil27hBK4RIN5_uG.0FL0MDOwwSO2kjMyEzW}
pvn.boklege{s5M-pVef0QPJil28hBK5RIO6_uG.0FM0MCOxvSO2jjNzEzV}
pvn.bolkdge{r4M-pUef0RPJil28gCL5RIN5_tH.0FL0LDOwvRO2kiNyDzW}
pvn.bolkege{r5M-oUdf0ROIil17hCK5QIO6_tH.0FL0LCOxwRO2jjMyEzW}
pvn.bollegd{s5M-pVdf0RPJil28hCK5RHN6_uH.0FM0MDOxvRO2kiNzDzW}
pvn.cnlkdfe{s5M-pUef0QPJil28hCL4RIO5_uG.0FL0MDOwvRN1jjNzEzV}
pvn.cnlldge{s5M-oVde0ROIhk17gCL4RIN6_tH.0FL0MDOxwSO1kjMzEzW}
pvn.cnlldge{s5M-pVee0RPJhk27gCK5RIO5_uH.0EL0MCOxwSO1jiMzEzW}
pvn.cokldge{s4M-oUee0RPJik27gBK5RIO5_uH.0EM0LDOwwRN2jjNzEzV}
pvn.coklefe{s5M-oUef0ROJil18hCL5RHN6_uH.0FM0MDNwwSO2kiMzEzW}
pvn.coklege{s4M-pUef0RPJil28gCL5RIO6_tH.0EM0LDNxwSO2jjNzEyV}
pvn.colkegd{s5M-pVef0RPIik17hBL5RIO6_tH.0FM0MCOxvSO1kjNyDyW}
pvn.colldge{s4L-pVef0QPJhk27hBL5RIN6_uH.0EM0MDOxvSN1jjNzEzV}
pvn.college{r5M-pVef0RPJil28gCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pvn.college{s4M-pUef0QOJik28gCK4QHO5_uG.0EM0LDOxvSN2jjNyEzW}
pvn.college{s4M-pVdf0RPJil28hCL5RHO6_uH.0FM0MDNxwSN2kiNyDzW}
pwm.cokldge{s5M-oVef0QOJil28gCL4RIO6_uH.0FL0MDOxwRN1kiMyDzW}
pwm.coklefd{s5L-pUef0QPJik18hBL4QIO6_uH.0FM0LCOxwSO2kjNzEyW}
pwm.colkefe{s4M-pUef0ROIhl17hCK4QIO5_uH.0FM0LDOxwSN1jjMzDzV}
pwm.colkege{s5L-pUef0RPJhl28hCL5RHO6_uH.0FM0MDOxwSN2kiMzEzW}
pwm.colkege{s5L-pVee0ROJik28hBK4RHO6_tH.0FM0MCOxwSO1kjNzDzW}
pwm.colkege{s5M-pVef0QPIik18hCL5RHO6_tH.0FM0LDOwvSO2kjNzEyV}
pwm.collefd{s5M-pVef0RPIil18hCK5RIO6_uG.0FM0MCNwwSO2kjNzEzW}
pwm.collefe{s5M-pVef0RPJil28hBL5RIO6_uH.0FM0MDOxwRO2kjNzEzW}
pwm.collegd{s5M-pVdf0QPJik27hCL5QIO5_tH.0EM0MDNxwSO1kiNyEzW}
pwm.college{s5M-pVef0RPJil28hCL5QHO6_uH.0FM0MDNxwSO2kjNzEzV}
pwn.bollegd{s5M-pVee0RPJhk18gCK5RIO5_uH.0EL0MCNxwRN2jjMzEyW}
pwn.bollege{s5L-pVef0RPJil18hCL4RIO6_tG.0EL0LCOwwSN2kjMyEzW}
pwn.cnkldge{s4M-pVef0RPJhk28hCK5RIO6_uH.0EL0MDNwwRO1kjNzEzW}
pwn.cnlldge{s4M-pVef0QPIik18gCL4RIO6_uH.0EM0LCNxwSO2kjMzEzV}
pwn.cokkege{r4M-pVdf0RPJil28hCL4RHO6_uH.0FM0MDOwwSO2jjNzEyW}
pwn.cokldge{s5M-pUdf0QOJik18hCL5QIO6_uH.0FM0MDOxvSO2kjMzDyW}
pwn.coklege{s5M-pVef0RPIik28hCL5RIO6_uH.0FM0MDOxwSO2kjNzEyW}
pwn.coklege{s5M-pVef0RPJil28hCL5RIN6_uH.0FM0LCOxwRO2kiNzDzW}
pwn.colkdfd{s5M-pVef0ROIil18gCK5RIO5_tH.0FM0MCNxwSO1jjMzEzV}
pwn.colkdge{s5L-pVef0RPJhk27hCL4RIN6_uH.0FM0MDNxwSN2kjNzEzW}
pwn.colkefe{r4L-oVef0RPIhl28hBL5QHO6_tG.0EM0LDNxwSO1kjNzEyW}
pwn.colkege{s5M-pUef0RPJil28hBK5QIO6_uH.0EM0MDOxwSO1kjNzEzW}
pwn.colldge{r5M-oVef0QPJil28hCL5RIN5_uG.0FL0MDOxwRO2jjNzDzV}
pwn.colldge{r5M-pVef0RPJil17gCL5QIN6_uH.0FL0LCNxwSO1kjNzEzV}
pwn.colldge{s5M-pVee0QOJhl18hCK5RHO6_uG.0FM0MDNxwSO2kjNzEzV}
pwn.colldge{s5M-pVef0RPIil28gCL5RIO6_uG.0FM0MCNwwRO2kiNzEyW}
pwn.colldge{s5M-pVef0RPJil28hCL5RIO6_uH.0FM0MCOxwSN2kjNzEzW}
pwn.collefd{s4M-pVef0RPJil27hCL4RIO6_uH.0EM0MDOwwSO2kjNzEzW}
pwn.collefe{r5L-oVef0RPJhk28hCL5QIO5_tG.0FL0MCNxvSN2kjNzEzW}
pwn.collefe{s4L-pVef0RPJil28hCL5QIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.collefe{s5M-oVef0RPJil28hCL5RHO5_uG.0FL0MDNxwSO2kjNyEyW}
pwn.collefe{s5M-pUef0RPJhk28hCL5RIO5_uG.0EM0MCOxwSO2kjNzDzW}
pwn.collefe{s5M-pVdf0RPJil28hCL5RIN6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.collegd{r5M-oUef0QOJhk17hCL5RIO5_uH.0EL0MDOxwSN2jiNzDzW}
pwn.collegd{r5M-pVef0RPJil28hCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{r4L-pVef0QPIil18hBK5RIN6_uH.0FM0LCOxwRO2jjNzDyV}
pwn.college{s4M-pUee0RPJil28hCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s4M-pVef0RPJil28hCL5RIO6_uG.0FM0MDOxwSO2kjNzDzW}
pwn.college{s4M-pVef0RPJil28hCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5L-pVef0RPJil18hCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5L-pVef0RPJil28hCL5RIO6_uH.0FM0MDOxwSO2jjNzEzW}
pwn.college{s5M-oUef0ROJil28hCL5RIO6_uG.0FM0MDOwvSO2kjNyDzW}
pwn.college{s5M-oVef0RPJil28gBL5QIN6_uH.0FM0MDOwwSO1jiNzDzW}
pwn.college{s5M-pUef0RPIil28hCL5RHO6_uH.0FL0MDOxwRN2kiNzEzW}
pwn.college{s5M-pUef0RPJil18hCL5RIN6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5M-pUef0RPJil28hCL4RIO6_tH.0FM0MDNxwSO2kjNyEzW}
pwn.college{s5M-pVdf0RPJil28hBL4RIO6_uH.0FM0MDOxwSO2jjNzDzW}
pwn.college{s5M-pVef0QPJil28hCL5RIO6_uH.0FM0MDOxwSO2kjMzEzW}
pwn.college{s5M-pVef0RPIil28hCL5RIO6_uH.0FM0MDOxwSO1kjNzEzW}
pwn.college{s5M-pVef0RPJik28hCK5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5M-pVef0RPJil28hBL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5M-pVef0RPJil28hCK5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5M-pVef0RPJil28hCL4RHO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5M-pVef0RPJil28hCL5QIO6_uH.0FM0MDOxwSO2kjNzEzW}
pwn.college{s5M-pVef0RPJil28hCL5RIO6_uH.0FM0MDOxwSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the sort command and how to sort data in the file.

### REFERENCES:
None. 
