# Reading Files
This challenge asks us to store the contents of the file `/challenge/read_me` to the `PWN` variable using read and then print it
```bash
Connected!
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{A9ONqlGpd7-68oVsfT-vZm8z6NX.dBjM4QDLzQjN1czW}
hacker@variables~reading-files:~$
```
I used the `<` to transfer the input of `/challenge/read_me` into `read PWN` command which gave me the flag
