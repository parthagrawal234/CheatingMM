# Groups and Files
This challenge asks to change the group of file `/flag` to hacker to access the file get the flag
```bash
Connected!
hacker@permissions~groups-and-files:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{Q_IQfsUFNacHa-_YhsLNp3Z2aQQ.dFzNyUDLzQjN1czW}
hacker@permissions~groups-and-files:~$
```
I used `chgrp` command to change the group of `/flag` to `hacker` then it can be accessed by the me to get the flag
