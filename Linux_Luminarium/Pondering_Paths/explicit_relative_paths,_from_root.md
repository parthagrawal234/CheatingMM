# Explicit Relative Paths, From /
This challenge asks us to invoke `run` using relative path using .
```bash
Connected!
hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{AbBRmCzp8PtpbH2auEvK5baHRVk.dBTN1QDLzQjN1czW}
hacker@paths~explicit-relative-paths-from-:/$
```
I have went into the `root` folder and then invoked relative path `./challenge/run`
