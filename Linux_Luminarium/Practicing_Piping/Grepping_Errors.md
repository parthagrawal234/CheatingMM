# Grepping Errors
This challenge asks us to pipe the error and output of `/challenge/run` and search it to get the flag
```bash
Connected!
hacker@piping~grepping-errors:~$ /challenge/run 2>&1 | grep "pwn.college"
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/xpq4yhadyhazkcsggmqd7rsgvxb3kjy4-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{4Wm_QJa-wBrnnDn4mEF2_6-BLif.dVDM5QDLzQjN1czW}
hacker@piping~grepping-errors:~$
```
I used the `2>&1` to make the redirect the file descriptor to another file descriptor which in this case is to `stderr` to `stdout` and grep it using the `|` to redirect the error to input 
