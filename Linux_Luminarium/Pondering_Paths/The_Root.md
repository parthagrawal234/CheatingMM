# The Root 
The challenge asks us to invoke the absolute path of the file `pwn`
```bash
hacker@paths~the-root:~$ ls
Desktop  n  not-the-flag
hacker@paths~the-root:~$ ls /
bin        dev   home   lib64   mnt  proc  run   sys  var
boot       etc   lib    libx32  nix  pwn   sbin  tmp
challenge  flag  lib32  media   opt  root  srv   usr
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{08YfBAVXeWZLYde35P-B_OzQYSd.dhzN5QDLzQjN1czW}
hacker@paths~the-root:~$
```
I first checked the path of the dir pwn and then invoked it using the command `/pwn`
