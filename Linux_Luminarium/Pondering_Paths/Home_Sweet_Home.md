# Home Sweet Home
This challenge asks us to copy the flag to any file as a argument of `/challenge/run` but the file should be inside `/home` directory and the path can only be 3 letter absolute path
```bash
Connected!
hacker@paths~home-sweet-home:~$ /challenge/run ~/r
Writing the file to /home/hacker/r!
... and reading it back to you:
pwn.college{MOIh1rL5hw4Sc1u3tY8DHio_yEq.dNzM4QDLzQjN1czW}
hacker@paths~home-sweet-home:~$
```
I invoked the absolute path of file r in `/home/hacker` in the argument of command of `/challenge/run` using the ~ symbol.
