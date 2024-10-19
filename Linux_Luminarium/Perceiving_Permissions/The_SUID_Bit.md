# The SUID Bit
This challenge asks us to add a `suid` permissions to `/challenge/getroot` to spawn a root shell to get the flag
```bash
Connected!
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ ls -l /challenge
total 16
-rwsr-xr-x 1 root root 1450 Aug 18 06:57 DESCRIPTION.md
drwsr-xr-x 2 root root 4096 Jul 19 20:31 bin
-rwsr-xr-x 1 root root  155 Jul 12 10:30 getroot
-rwsr-xr-x 1 root root   43 Feb  8  2024 run
hacker@permissions~the-suid-bit:~$ sudo cat /flag
sudo: workspace is not privileged
hacker@permissions~the-suid-bit:~$ /challenge/getroot cat /flag
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{4NPpLV3DGbZwRJkR1jbo8RlDAZo.dNTM2QDLzQjN1czW}
root@permissions~the-suid-bit:~#
```
I used `chmod` to give suid bit to `/challenge/getroot` and invoked it to become root and then used `cat /flag` to get the flag
