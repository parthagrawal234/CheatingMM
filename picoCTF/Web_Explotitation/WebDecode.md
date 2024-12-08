# Web Decode
This challenge tests our basic searching skills on a inspect of a website to find the flag

## Website Provided
[Click_Here](http://titan.picoctf.net:62401)

## Hints Given
Hint 1: Use the Web Inspector on other pages of the website

Hint 2: The Flag may or may not be encoded

## Procedure
1. I opened the website and Opened the inspect animation on the Home Page and Used the Search to find the flag found nothing
2. I tried to find the flag Manually in encoded as mentioned in Hint 2
3. After that i switched to the About Page Where it said that the flag is in there and we have to check

![image](https://github.com/user-attachments/assets/87dcfb39-25b3-4680-8efb-b58d428c2221)

4. I could not find anything except this gibberish written in the section folder named `cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfMDdiOTFjNzl9`

![image](https://github.com/user-attachments/assets/c5087cb7-2900-49aa-8199-9003f10a728d)

5. Using [Cryptii](https://cryptii.com/pipes/caesar-cipher) I tried every combination till i found `Base64` which gave me my flag

## Flag
`picoCTF{web_succ3ssfully_d3c0ded_07b91c79}`
