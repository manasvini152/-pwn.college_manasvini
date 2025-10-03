# **DATA MANIPULATION**
## **<ins>EXTRACTING SPECIFIC SECTIONS OF TEXT</ins>**
The cut command extracts particular columns of the text and prints it.

### SOLVE: 
***FLAG:*** pwn.college{Y38c_GVFWi_5p69CQwZGqayNp13.01NxEzNxwSO2kjNzEzW}

We use the command  /challenge/run | cut -d " " -f 2 | tr -d "\n".
Here we pipe throught /challenge/run. When we execute only /challenge/run the first column comprises of numbers and second column comprises
of characters. Hence we only need the second column. The numbers and characters are separated with the help of a " ".
Hence we use the column delimiter which specifies the separation. And we use -f 2  which specifies the column to be printed.
Now since each character of the flag is in a new line we use the tr -d "\n" command to delete the new lines.
Hence we obtain the flag.

```
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{Y38c_GVFWi_5p69CQwZGqayNp13.01NxEzNxwSO2kjNzEzW}
```

### WHAT I LEARNED: 
I learnt about the cut command and how to print a specific column.

### REFERENCES:
None. 
