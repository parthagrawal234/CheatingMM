# Writing to Multiple Programs
This challenge asks us to duplicate the output to input of two programs at the same time
```bash
Connected!
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack > >(/challenge/the | /challenge/planet)
Are you sure you're properly redirecting input into '/challenge/planet'?
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack > >(/challenge/the) | /challenge/planet
Are you sure you're properly redirecting input into '/challenge/planet'?
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack > >(/challenge/the) >(/challenge/planet)
Are you sure you're properly redirecting input into '/challenge/planet'?
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack > >(/challenge/the) /challenge/planet
hacker@piping~writing-to-multiple-programs:~$ cat /challenge/planet
#!/opt/pwn.college/bash

read CORRECT < /challenge/.challenge-key
read ATTEMPT < <(tail -n 1)

if [ "$CORRECT" == "$ATTEMPT" ]
then
        echo "$CORRECT" > /challenge/.planet
else
        fold -s >&2 <<< "Are you sure you're properly redirecting input into '/challenge/planet'?"
fi
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
321602063155238036
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{88GJb9Pw4o3cWQsdm_r5kCLsC6N.dBDO0UDLzQjN1czW}
hacker@piping~writing-to-multiple-programs:~$
```
I used the tee command to duplicate the output of the command `/challenge/hack` and then `>()` to create two tmp file of `/challenge/the` and `/challenge/planet` 
