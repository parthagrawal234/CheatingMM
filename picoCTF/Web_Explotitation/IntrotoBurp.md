# Intro to Burp
This challenge allows us to use a proxy server to interpret the websites input and outputs to find the flag

## Website Provided
[Click_Here](http://titan.picoctf.net:62453/)

## Hints Given
Hint 1: Try using burpsuite to intercept request to capture the flag

Hint 2: Try mangling the request, maybe their server-side code doesn't handle malformed requests very well

## Procedure
1. In BurpSuite I opened the wesbite using its proxy server and intercepted the request for a `GET` which i forwarded
2. This opened the request for a some username and password which i entered at random
   
![image](https://github.com/user-attachments/assets/0c052fc0-a73e-4491-8d79-dc7c74b89710)

3. This opened a `POST` and a `GET` request on the server which i forwarded and found it asking for a OTP

![image](https://github.com/user-attachments/assets/b46d3a48-0648-4d0e-9fc3-6335fb8ca0fc)

![image](https://github.com/user-attachments/assets/5d3974a0-7c47-4cd4-98b3-cb674bfc05db)

4. I entered a random OTP but showed a `Invalid OTP`.
   
![image](https://github.com/user-attachments/assets/bbadd0dc-facb-4544-9fea-e3e738918f05)

5. Rerunning the wesbsite i looked at the `POST` request again an found the `otp` input

![image](https://github.com/user-attachments/assets/be9bca73-3d54-48a3-9006-4bf78cb5591b)

6. I changed the otp to empty but still gave me wrong output
7. I realized to remove the input as it was not working correctly to the `Post` and I bypassed the request

![image](https://github.com/user-attachments/assets/ed8367ed-b2e5-4b4e-9b4c-6236210d0281)

## Flag Given
`picoCTF{#0TP_Bypvss_SuCc3$S_e1eb16ed}`
