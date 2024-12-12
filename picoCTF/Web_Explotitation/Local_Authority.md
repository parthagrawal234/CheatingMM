# Local Authority
This challenge makes us exploit the username and password gaps in the system and find the write username and password to find the flag

## Website Provided
[Click Here](http://saturn.picoctf.net:58572)

## Procedure
1. When i open the website I find the webpage with a local username and password login page

![image](https://github.com/user-attachments/assets/06dc5934-a9f8-4445-a059-2382f67c762b)

2. I use the inspector to see the script where it makes a `POST` request to the `login.php` on sign in which checks the valididity of the login details

![image](https://github.com/user-attachments/assets/0fde4153-29a9-4957-8ffa-23955337883e)

3. I use the random username and password to get to the login.php which showed login failed

![image](https://github.com/user-attachments/assets/5114e05f-bd74-4e8c-8511-158ea0265b6e)

4. I see the inspector that the system when the username and password is correct makes a `POST` request to `admin.php` and check the password and username with a function `checkPassword` which is taken from a external script `secure.js`

![image](https://github.com/user-attachments/assets/0e3c78fc-be21-4b6b-a8ca-06afa6acc409)

![image](https://github.com/user-attachments/assets/83361a58-ca5c-4816-94ee-e144b7051d26)

5. I tried to enter the `admin.php` directly but was given not authorized message as expected so i opened the `secure.js` file to check for the username and password

![image](https://github.com/user-attachments/assets/efe52575-a4e3-4793-819d-acfd25f43662)

![image](https://github.com/user-attachments/assets/3255285a-090e-498e-be37-c6a2639bf2fd)

6. I found the id and password as `admin` and `strongPassword098765` which when entering on the main page gave me access to `admin.php`

![image](https://github.com/user-attachments/assets/a7895421-cee7-47cf-96d6-985b3bfe648c)

## Flag Provided
`picoCTF{j5_15_7r4n5p4r3n7_05df90c8}`
