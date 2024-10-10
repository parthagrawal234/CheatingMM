# Help for Builtins
This challenge asks us to use the `help` command to see the builtin shell documentation of `challenge` and then use the write argument to get the flag
```bash
Connected!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "oGPtj6rh".
hacker@man~help-for-builtins:~$ /challenge/challenge --secret oGPtj6r
h
ssh-entrypoint: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ challenge --secret oGPtj6rh
Correct! Here is your flag!
pwn.college{oGPtj6rhcLbOYDa_PV1XocWoXI6.dRTM5QDLzQjN1czW}

hacker@man~help-for-builtins:~$
```
I used the `help challenge` command to see the documentation and found the argument `--secret VALUE` which will print the flag for the correct value of VALUE and then found the correct value written below which was "oGPtj6rh"

Then I used the command `challenge --secret oGPtj6rh` to get the flag 
