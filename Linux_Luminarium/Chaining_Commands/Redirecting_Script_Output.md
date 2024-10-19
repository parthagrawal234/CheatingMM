# Redirecting Script Output
This challenge asks us to pipe the output of `chained /challenge/pwn and /challenge/college` script to `/challenge/solve` command to get the flag
```bash
Connected!
hacker@chaining~redirecting-script-output:~$ nano x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{4OqgOSCJlBQXv3hRW-ojhewydaa.dhTM5QDLzQjN1czW}
hacker@chaining~redirecting-script-output:~$
```
I used a script `x.sh` to chain `/challenge/pwn` and `/challenge/college` and pipe its output to `/challenge/solve` to get the flag
