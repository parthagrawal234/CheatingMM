# Exploring Variables
This challenge asks us to export the variable `PWN` with value COLLEGE and define a variable `COLLEGE` with valur PWN and not export it to get the flag
```bash
Connected!
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
Incorrect...
You have not set the COLLEGE variable to the correct value (it should be
'PWN'). Do that before running this script! Even though it is not exported, in
this challenge, we have ways to check...
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{cgKg61EoN72y6k47soDhYiewHP9.dJjN1QDLzQjN1czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$
```
I invoked the `/challenge/run` command to get the flag
