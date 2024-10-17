# Executable Files
This challenge asks you to change the permission of `/challenge/run` to be able to execute to get the flag
```bash
Connected!
hacker@permissions~executable-files:~$ /challenge/run
ssh-entrypoint: /challenge/run: Permission denied
hacker@permissions~executable-files:~$ chmod o+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
ssh-entrypoint: /challenge/run: Permission denied
hacker@permissions~executable-files:~$ ls -l /challenge/run
-r--r--r-x 1 hacker hacker 32 Jul  4 06:37 /challenge/run
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{0b8uWOb0pXwXefi8UYprifai_Xq.dJTM2QDLzQjN1czW}
hacker@permissions~executable-files:~$
```
I used `chmod u+x /challenge/run` to change the permission of the current user of the file as the user was hacker to be able to execute it to get the flag
