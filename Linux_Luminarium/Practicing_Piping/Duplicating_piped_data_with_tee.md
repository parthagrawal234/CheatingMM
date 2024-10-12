# Duplicating Piped Data with Tee
This challenge asks us to pipe the output of `/challenge/pwn` command to `/challenge/college` command but you need to intercept the data to see what is the error of commands
```bash
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee log | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat log
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "EpA5QF9R"
hacker@piping~duplicating-piped-data-with-tee:~$  /challenge/pwn --ecret EpA5QF9R | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{EpA5QF9R0wrJlEEDOMNk4uA7Ji3.dFjM5QDLzQjN1czW}
hacker@piping~duplicating-piped-data-with-tee:~$
```
I used the `tee` command to intercept the output of `/challenge/pwn` on to the log file and then read the file to see what arguments to pass then pipe the `/challenge/pwn` to `/challenge/college` command
