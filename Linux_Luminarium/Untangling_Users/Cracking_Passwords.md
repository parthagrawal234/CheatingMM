# Cracking Passwords
This challenge asks to crack the password of `zardus` using `John The Ripper` in the leaked version of `/etc/shadow` in `/challenge/shadow-leak`
```bash
Connected!
hacker@users~cracking-passwords:~$ john /etc/shadow
Created directory: /home/hacker/.john
fopen: /etc/shadow: Permission denied
hacker@users~cracking-passwords:~$ ls ~/.john
hacker@users~cracking-passwords:~$ ls -a ~
.              .bash_history  .cache   .john     .profile  PWN           myflag        r
..             .bash_logout   .config  .lesshst  COLLEGE   instructions  n             the-flag
.ICEauthority  .bashrc        .dbus    .local    Desktop   log           not-the-flag
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:12 0% 2/3 0g/s 285.2p/s 285.2c/s 285.2C/s brenda..keith
0g 0:00:00:13 0% 2/3 0g/s 286.0p/s 286.0c/s 286.0C/s serena..88888888
0g 0:00:00:16 0% 2/3 0g/s 286.5p/s 286.5c/s 286.5C/s rockie..surfing
0g 0:00:00:18 1% 2/3 0g/s 286.8p/s 286.8c/s 286.8C/s chacha..jazmin
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04926g/s 286.8p/s 286.8c/s 286.8C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{8axOabt9cx6A0RYqaK8ToWoJ__c.ddTN0UDLzQjN1czW}
zardus@users~cracking-passwords:/home/hacker$
```
I used `john /challenge/shadow-leak` to crack the password as `aadvark` and got access to `zardus` to get the flag
