# Searching Manuals
This challenge asks us to search the manual of `challenge` using the `man` commands and arguments `/,n,N,?`
```bash
Connected!
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --kz
Initializing...
Correct usage! Your flag: pwn.college{gvErSR3QN_QLAoRkDTt-Pxtd_vr.dVTM4QDLzQjN1czW}
hacker@man~searching-manuals:~$
```
I read the documentation and tried to press `return` to read line by line but then i couldn't find it so i used `/flag` to search for the keyword flag in the manual i got flag in the title of the file so i pressed `n` to go to next result to `--kz` argument in the 1123 line that will give me the flag.<br />
<br />
After that i used the command `/challenge/challenge --kz` to get the flag
