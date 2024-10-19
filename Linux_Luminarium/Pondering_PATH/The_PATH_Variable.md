# The PATH Variable
This challenge asks us to make the `PATH` variable to remove all the commands direct paths so that u can't name call them and then use `/challenge/run` to get the flag
```bash
Connected!
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{s77dzklLOAls7x36VWCCo_hd33a.dZzNwUDLzQjN1czW}
hacker@path~the-path-variable:~$
```
I used Shell Variables to make the variable `PATH` empty so that `/challenge/run` cant run the `rm` command then used it to get the flag
