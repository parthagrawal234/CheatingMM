# Starting Background Processes
This challenge asks you to start the process `/challenge/run` from the background to get the flag
```bash
Connected!
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 82



Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{c2lACjM7V50Kz3nJFv3D1dXZJfc.dlDN4QDLzQjN1czW}
[1]+  Done                    /challenge/run
hacker@processes~starting-backgrounded-processes:~$
```
I used `&` operator in front of `/challenge/run` to run it in the background and get the flag
