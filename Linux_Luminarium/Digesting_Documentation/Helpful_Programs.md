# Helpful Programs
This challenge asks us to use `--help` argument to command `/challenge/challenge` to see what to do to get the flag
```bash
Connected!
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g
                        option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -g GIVE_THE_FLAG
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: invalid int value: 'GIVE_THE_FLAG'
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 141
hacker@man~helpful-programs:~$ /challenge/challenge -g 141
Correct usage! Your flag: pwn.college{oXdN_VPawKgUl-FuwdM-1NHmfwA.ddjM4QDLzQjN1czW}
hacker@man~helpful-programs:~$
```
I used the `/challenge/challenge --help` to find that `-g GIVE_THE_FLAG` gives the flag if you put the right value of GIVE_THE_FLAG and to find that right value we use `-p` argument to `/challenge/challenge`

So I used the command `/challenge/challenge -p` to get the right value which was 141 then used the command `/challenge/challenge -g 141` to get the flag
