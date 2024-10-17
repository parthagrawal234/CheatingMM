# Changing Permissions
This challenge asks to give read permissions to hacker of the file `/flag` to get the flag
```bash
Connected!
hacker@permissions~changing-permissions:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~changing-permissions:~$ chmod o+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{oyU15qMhhLVD17tBqg8sYxLJr75.dNzNyUDLzQjN1czW}
hacker@permissions~changing-permissions:~$
```
I used the `chmod o+r /flag` to add read permission to all the users then used `cat` to read the flag
