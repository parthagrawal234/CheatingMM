# Matching with *
This challenges asks us to cd into the `/challenge` directory with only four or less character in the argument
```bash
nnected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /*c*
ssh-entrypoint: cd: too many arguments
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ ./run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{oo6UlGIO8H50os5I6uOnQHlNPKp.dFjM4QDLzQjN1czW}
hacker@globbing~matching-with-:/challenge$
```
I used the `*` operator to make the challenge short like `/c*` and then used the command `cd /c*` to cd into challenge

Then I used `./run` to get the flag
