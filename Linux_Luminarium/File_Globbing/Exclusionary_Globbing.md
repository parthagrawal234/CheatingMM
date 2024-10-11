# Exclusionary Globbing
This challenge asks us to go the `/challenge/files` and read the files not starting with [pwn] to get the flag
```bash
Connected!
hacker@globbing~exclusionary-globbing:~$ /challenge/run /challenge/files [!pwn]*
Error: please run with a working directory of /challenge/files!
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{YeMXL0PvISBaS5ZMNJkzROBWOIQ.dZjM4QDLzQjN1czW}
hacker@globbing~exclusionary-globbing:/challenge/files$
```
