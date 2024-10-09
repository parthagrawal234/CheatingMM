# Implicit relative paths, from /
The challenge asks us to invoke the implicit relative path of `run` from a dir so that the relative path starts from c
```bash
Connected!
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ ./challenge/run
Incorrect...
This challenge must be invoked with a relative path that starts with a letter!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{oCvMyALlcuKUml5r3XpspmPX8e4.dlDN1QDLzQjN1czW}
hacker@paths~implicit-relative-paths-from-:/$
```
I knew from the hint that the path start from challenge so we need `cd` into root folder and invoke `challenge/run` path
