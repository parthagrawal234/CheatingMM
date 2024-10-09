# Position Elsewhere
This challenge asked us to `cd` into a specific dir and run `/challenge/run` from it
```bash
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/include directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/include
hacker@paths~position-elsewhere:/usr/include$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{0gQBaRsRTjDko31wYzH5qkZJEoP.ddDN1QDLzQjN1czW}
hacker@paths~position-elsewhere:/usr/include$
```
I have `cd`ed into the `/usr/include` directory and invoked `/challenge/run` from there
