# The First Shell Script
This challenge asks us to write a shell script and run it to get the flag
```bash
Connected!
hacker@chaining~your-first-shell-script:~$ bash x.sh
bash: x.sh: No such file or directory
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ nano x.sh
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ nano x.sh
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{ohl_RB1-hXgiMSBpcPts_cIELgS.dFzN4QDLzQjN1czW}
hacker@chaining~your-first-shell-script:~$
```
I used `touch` and `nano`to make this file and then used `bash x.sh` to get the flag
