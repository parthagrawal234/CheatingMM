# Redirecting Input
This challenge asks us to redirect the contents of file `pwn` to `/challenge/run` as input and then run it to get the flag
```bash
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{sNyVGBFP6dQF6SRNU6jVCb8F6Oe.dBzN1QDLzQjN1czW}
hacker@piping~redirecting-input:~$
```
I used `echo COLLEGE > pwn` to write the correct input to PWN file and then used `<` command to redirect the contents of PWN to `/challenge/run` command and get the flag
