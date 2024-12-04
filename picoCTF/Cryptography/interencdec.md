# Interendec
This challenge is a simple multiple encoding challenge and is required to decode into a flag.

## File Provided
[enc_flag.txt](https://github.com/user-attachments/files/18006488/enc_flag.txt)


## Base64 Encoding
The file provided opens up to the encoded string `YidkM0JxZGtwQlRYdHFhR3g2YUhsZmF6TnFlVGwzWVROclh6YzRNalV3YUcxcWZRPT0nCg==` which looks like a base64 encoding due `==` signs at the end. 
Decryting it makes it `b'd3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzc4MjUwaG1qfQ=='`. 

Removing the `b` and `''` makes it another Base64 encoding which is decrypted to `wpjvJAM{jhlzhy_k3jy9wa3k_78250hmj}` which kind of looks like a flag with a ceaser cipher

## Caesar Cipher
When `wpjvJAM{jhlzhy_k3jy9wa3k_78250hmj}` is decoded with a shift of 7 in caesar cipher the text is decoded as `picoCTF{caesar_d3cr9pt3d_78250afc}` which is the flag.
