# Killing Processes
This challenge asks us to terminate the program `/challenge/dont_run` so that `/challenge/run` runs
```bash
Connected!
hacker@processes~killing-processes:~$ ps -ef | grep /challenge/dont_run
hacker        73      71  0 09:45 ?        00:00:00 /challenge/dont_run
hacker        93      75  0 09:45 pts/0    00:00:00 grep --color=auto /challenge/dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{IE6qEQv9S8Y2rQ1GwwoFcuSB9eR.dJDN4QDLzQjN1czW}
hacker@processes~killing-processes:~$
```
I used the `ps -ef` command and piped its output into `grep` to find `/challenge/dont_run` command's PID code

Then I used the `kill` command to terminate the process and then used `/challenge/run` to get the flag
