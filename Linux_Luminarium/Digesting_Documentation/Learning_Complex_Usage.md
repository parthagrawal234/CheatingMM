# Learning Complex Usage
This challenge asks us to invoke the `/challenge/challenge` with its argument `--printfile` to print the contents of an arbitary file
```bash
Connected!
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{0mP6-sa7d6Kxtclo18OrINC_TPJ.dVjM5QDLzQjN1czW}
hacker@man~learning-complex-usage:~$
```
I used this documentation for `/challenge/challenge` function <br />
<br />
Welcome to the documentation for `/challenge/challenge!` This program allows you to print arbitrary files to the terminal, when given the `--printfile` argument. The argument to the `--printfile` argument is the path of the flag to read. For example, `/challenge/challenge --printfile /challenge/DESCRIPTION.md` will print out the description of the level!<br />
<br />
I used this documentation to invoke the `/challenge/challenge --printfile /flag` command as I know that flag is mostly in `/flag` in the challenges
