# Reading Input
This challlenge asks us to read the value from the user and store it in a variable `PWN` to get the flag
```bash
Connected!
hacker@variables~reading-input:~$ read "Input: " PWN
ssh-entrypoint: read: `Input: ': not a valid identifier
hacker@variables~reading-input:~$ read -p "Input: " PWN
Input: COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{keyPPGtfNpN2ehjxcTryPuD26Qv.dhzN1QDLzQjN1czW}
hacker@variables~reading-input:~$
```
I used the `read` command to get input from the user of the value `COLLEGE` to get the flag
