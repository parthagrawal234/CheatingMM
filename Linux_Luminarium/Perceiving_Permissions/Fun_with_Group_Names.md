# Fun with Group Names
This challenge asks to change the group of `/flag` to a special group name `hacker` user is in
```bash
Connected!
hacker@permissions~fun-with-groups-names:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp4278) groups=1000(grp4278)
hacker@permissions~fun-with-groups-names:~$ chgrp grp4278 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{sqh9Nr1l5CXE-L14k1KIpfkcgnb.dJzNyUDLzQjN1czW}
hacker@permissions~fun-with-groups-names:~$
```
I used the `id` command to find the group hacker is in then used the `chgrp grp4278 /flag` command to change the group of `/flag` to get the flag
