# Redirecting More Output 
This challenge asks us to redirect the output of the command `/challenge/run` to `myflag` file to get the flag
```bash
Connected!
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oJISKeWS-dhJwg3pGaqGC2QQxAq.dVjN1QDLzQjN1czW}

hacker@piping~redirecting-more-output:~$
```
I used the `>` to redirect the output of `/challenge/run` command to the myflag file and used `cat` to read the file to get the flag
As I used the command I saw it showing the whole process 
