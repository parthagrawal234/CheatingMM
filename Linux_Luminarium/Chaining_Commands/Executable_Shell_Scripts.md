# Executable Shell Scripts
This challenge asks us to write a script and then make it executable to directly run to get the flag
```bash
Connected!
hacker@chaining~executable-shell-scripts:~$ nano x.sh
hacker@chaining~executable-shell-scripts:~$ chmod u+x x.sh
hacker@chaining~executable-shell-scripts:~$ ./x.sh
Congratulations on your shell script execution! Your flag:
pwn.college{Qu8qiE6ouAbwwOncNRv75kxwgbr.dRzNyUDLzQjN1czW}
hacker@chaining~executable-shell-scripts:~$
```
I made a `x.sh` script with `/challenge/solve` command in it and then made it executable using `chmod` then executated it using `./x.sh` to get the flag
