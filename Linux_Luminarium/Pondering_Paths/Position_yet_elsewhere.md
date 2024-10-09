# Position Yet Elsewhere
This challenge asks us to invoke `/challenge/run` from a specific dir it asks us to go into using `cd`
```bash
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /tmp
hacker@paths~position-yet-elsewhere:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wXRDNm5YDchCKNiZtuNzPEMICSL.dhDN1QDLzQjN1czW}
hacker@paths~position-yet-elsewhere:/tmp$
```
I `cd`ed into the `/tmp` and then invoked `/challenge/run` dir
