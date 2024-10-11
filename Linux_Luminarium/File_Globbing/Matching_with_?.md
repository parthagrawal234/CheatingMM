# Matching with ?
This challenge asks us to cd into challenge by using the `?` in the path of the file to replace the text
```bash
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ ./run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{8YgHuSawk6lQB4CT2grZMhYelUs.dJjM4QDLzQjN1czW}
hacker@globbing~matching-with-:/challenge$
```
I wrote the command `cd /?ha??enge` to cd in the `/challenge` directory and then `./run` to get the flag
