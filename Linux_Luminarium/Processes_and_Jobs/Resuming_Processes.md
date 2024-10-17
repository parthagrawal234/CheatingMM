# Resuming Process
This challenge asked as to suspend `/challenge/run` and then resume it to get the flag
```bash
Connected!
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{AP02WlY2GJaN3L76iBMeoJdNsVN.dZDN4QDLzQjN1czW}
Don't forget to press Enter to quit me!
```
I used `Ctrl-Z` to first suspend the command after running it then used `fg` command to resume it back to get the flag
