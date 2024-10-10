# Reading Manuals
This challenge asks us to read the manual of `/challenge/challenge` command using the `man` command and find the secret argument to print the flag
```bash
Connected!
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)             Challenge Commands             CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --lmalpw NUM
              print the flag if NUM is 015

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The  repository  for  this  dojo: <https://github.com/pwncol‐
       lege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                   May 2024                  CHALLENGE(1)
hacker@man~reading-manuals:~$ challenge --lmalpw 015
ssh-entrypoint: challenge: command not found
hacker@man~reading-manuals:~$ /challenge/challenge --lmalpw 015
Correct usage! Your flag: pwn.college{0LX15WOVlPUC_KmBalp6BMDCA9w.dRTM4QDLzQjN1czW}
hacker@man~reading-manuals:~$
```
I read the whole manual of `challenge` using the `man challenge` command and then the command is `/challenge/challenge` and the secret argument is `--lmalpw NUM` but it will only give the flag when NUM=015.<br />
<br />
Therefore I give the command `/challenge/challenge --lmalpw 015` to get the flag
