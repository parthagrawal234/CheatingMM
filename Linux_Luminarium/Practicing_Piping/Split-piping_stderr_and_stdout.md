# Split-piping stderr and stdout
This challenge asks us to pipe the error of `/challenge/hack` into `/challenge/the` and and pipe output into `/challenge/planet` without mixing them 
```bash
Connected!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{4rlixSVyCAo4xy7uPsubXIxOR5D.dFDNwYDLzQjN1czW}
```
I used the command `/challenge/hack 2> >(/challenge/the) | /challenge/planet` to get the flag
