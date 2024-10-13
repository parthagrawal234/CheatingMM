# Storing Command Output
This challenge asks us to store the output of `/challenge/run` commands to `PWN` variable to get the flag
```bash
Connected!
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo &PWN
[1] 93

[1]+  Done                    echo
ssh-entrypoint: PWN: command not found
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{sgLmkssE_XlAF96gX6HQxLll_GG.dVzN0UDLzQjN1czW}
hacker@variables~storing-command-output:~$
```
I used the command `PWN=$(/challenge/run)` to store the flag in the output of `/challenge.run` on `PWN` and then printed it to get the flag
