# Redirecting Errors
This challenge asks us to redirect the output of `/challenge/run` command to myflag file and errors to the instructions file and then read the myflag file to get the flag
```bash
Connected!
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ ./instructions
ssh-entrypoint: ./instructions: Permission denied
hacker@piping~redirecting-errors:~$ ls
COLLEGE  Desktop  instructions  myflag  n  not-the-flag  r  the-flag
hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{gYg6E_90tcvp4D7jE6Eh2RpDZt6.ddjN1QDLzQjN1czW}

hacker@piping~redirecting-errors:~$
```
I used the `>` and `2>` commands to redirect the output and errors of to myflag and instructions files and then used to `cat` to read instruction file to see if transfer was a success and then opened the myflag file using `cat` to get the flag
