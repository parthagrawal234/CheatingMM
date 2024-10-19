# Setting PATH
This challenge asks to overwrite the `PATH` variable by the path of the win command and use `/challenge/run` to get the flag
```bash
Connected!
hacker@path~setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{4VaCaH_HqDAbrpd_QGLShZeVRMt.dVzNyUDLzQjN1czW}
hacker@path~setting-path:~$
```
I set the variable PATH to `/challenge/more_commands` which has the win command so that when `/challenge/run` calls it can refer the variable to use the command
