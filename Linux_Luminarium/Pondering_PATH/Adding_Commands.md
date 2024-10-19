# Adding Commands
This challenge asks us to add the win command to `PATH` variable using shell script then use it to run `/challenge/run` to get the flag
```bash
Connected!
hacker@path~adding-commands:~$ PATH+=:/home/hacker
hacker@path~adding-commands:~$ chmod ugo+x ./win
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{4I3zpBw0vAracbXr_JrO9e9rWAm.dZzNyUDLzQjN1czW}
hacker@path~adding-commands:~$
```
I made a file `win` in `/home/hacker` then gave it execute permission using `chmod` then appended `/home/hacker` into the `PATH` variable then executed the `/challenge/run` command
