# Listing Processes
This challenge asks us to find the `/challenge` command without using `ls`
```bash
Connected!
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 04:46 ?        00:00:00 /sbin/docker-init
root           7       1  0 04:46 ?        00:00:00 /run/dojo/bin/slee
root          68       1  0 04:46 ?        00:00:00 /challenge/14143-r
root          72      68  0 04:46 ?        00:00:00 sleep 6h
hacker        73       0  0 04:47 pts/0    00:00:00 /run/dojo/bin/ssh-
hacker        90       0  0 04:48 pts/1    00:00:00 /run/dojo/bin/ssh-
hacker       107      90  0 04:49 pts/1    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/14143-r
ssh-entrypoint: /challenge/14143-r: No such file or directory
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   04:46   0:00 /sbin/docker-init -- /nix/var/nix/profiles/
root           7  0.0  0.0   5052  2240 ?        S    04:46   0:00 /run/dojo/bin/sleep 6h
root          68  0.0  0.0   4132  2560 ?        S    04:46   0:00 /challenge/14143-run-3360
root          72  0.0  0.0   2744  1600 ?        S    04:46   0:00 sleep 6h
hacker        73  0.0  0.0   5240  3840 pts/0    Ss+  04:47   0:00 /run/dojo/bin/ssh-entrypoint
hacker        90  0.0  0.0   5372  3840 pts/1    Ss   04:48   0:00 /run/dojo/bin/ssh-entrypoint
hacker       109  0.0  0.0   7868  3200 pts/1    R+   04:51   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/14143-run-3360
Yahaha, you found me! Here is your flag:
pwn.college{ckollcxNl6FwK-xtHgaE0OH22q8.dhzM4QDLzQjN1czW}
Now I will sleep for a while (so that you could find me with 'ps').
```
I used `ps aux` to find `/challenge/14143-run-3360` and ran to get the flag
