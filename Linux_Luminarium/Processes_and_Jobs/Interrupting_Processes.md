# Interrupting Processes
This challenge asks to intterupt the process `/challenge/run` while it is running in the terminal
```bash
Connected!
hacker@processes~interrupting-processes:~$ ^C
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{IwLBmbuaKBq2ejVgDE3zsuGUWC4.dNDN4QDLzQjN1czW}
```
I used `Ctrl-C` to terminate the process while it was running in the terminal to get the flag
