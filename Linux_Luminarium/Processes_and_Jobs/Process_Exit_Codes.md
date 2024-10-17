# Process Exit Codes
This challenge asks us to find the error exit code of `/challenge/get-code` command and then use it as an argument in `/challenge/submit-code` to get the flag
```bash
Connected!
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
141
hacker@processes~process-exit-codes:~$ /challenge/submit-code 141
CORRECT! Here is your flag:
pwn.college{ADwUlPqhVxSprLyfHs9_A1kntjx.dljN4UDLzQjN1czW}
hacker@processes~process-exit-codes:~$
```
I used the `?` variable to read the value of the exit code after running the command `/challenge/get-code` and then used the command `/challenge/submit-code` to get the flag
