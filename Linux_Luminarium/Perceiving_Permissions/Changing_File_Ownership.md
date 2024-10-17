# Changing File Ownership
This challenge asks us to change the ownership of file `/flag` to `hacker` then cat it as a user to get the flag
```bash
Connected!
hacker@permissions~changing-file-ownership:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{4WA8wXOtw2aXhknCFryaPqu_6QC.dFTM2QDLzQjN1czW}
hacker@permissions~changing-file-ownership:~$
```
I used chown to change the ownership of `/flag` from `root` to `hacker` then used `cat /flag` to get the flag 
