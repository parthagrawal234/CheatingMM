# Implicit Relative Path
This challenge asks us to invoke relative path of `run` from `/challenge` directory
```bash
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cTCfEgx-6IehOWk5Tbp5IzaiNNl.dFTN1QDLzQjN1czW}
hacker@paths~implicit-relative-path:/challenge$
```
I have `cd`ed into the `/challenge` directory and then invoke the relative path by `./run`
