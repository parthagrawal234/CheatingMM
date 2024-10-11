#Mixing Globs
This challenge asks us to run the files pwning, challenging and educational with only 6 arguments using globs
```bash
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *n*
Error: you did not use a square bracket glob...
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *n*[gl]
Error: your argument is too long! It must be 6 characters or less.
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *[gl]
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
amazing beautiful challenging delightful educational jovial laughing magical pwning thrilling uplifting wonderful xenial youthful
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *n[gl]
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
amazing challenging laughing pwning thrilling uplifting
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run ?[hdw]
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
?[hdw]
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run ?[hdw]*
Error: your argument is too long! It must be 6 characters or less.
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cpe]*
You got it! Here is your flag!
pwn.college{88wcvexfla2D-WIU4urEkP7ekxD.dVjM4QDLzQjN1czW}
hacker@globbing~mixing-globs:/challenge/files$
```
I tried to find same letters in the same place in the words but couldn't file any then found that starting letters of files are unique to then so I used the command `/challenge/run [cpe]*` to get the flag
