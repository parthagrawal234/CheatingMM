# RSA Oracle
This challenge gives us a encrypted flag with a password to decrypt but the password is also encrypted

## Files Provided
[secret.enc](https://artifacts.picoctf.net/c_titan/32/secret.enc)

[password.enc](https://artifacts.picoctf.net/c_titan/32/password.enc)

## Hints Given
-Hint 1: Crytography Threat models: chosen plaintext attack.

-Hint 2: OpenSSL can be used to decrypt the message. e.g ```openssl enc -aes-256-cbc -d ...```

-Hint 3: The key to getting the flag is by sending a custom message to the server by taking advantage of the RSA encryption algorithm.

-Hint 4: Minimum requirements for a useful cryptosystem is CPA security.

## Password Decryption
The Password file is given as a digit of long numbers which means it is `RSA` encrypted and without the private key cannot be unlocked but the challenge has also provided us with a software which will encrypt and decrypt any data with the same `e, d and n` except the password

So first we encrypt the data with a ASCII value of `20` in hex which is space whose encrypted value is `20^e mod n` which is `3970921715843088939034957324911350626212240950470862928977787663977406608468604142079377234654007309935996972791790270166961305129444105909465676647301056`

We multiply this number by our password encrypted number `1765037049764047724348114634473658734830490852066061345686916365658618194981097216750929421734812911680434647401939068526285652985802740837961814227312100` which gives us `7008823950175675948553224791235929059908363653777472741201303682989871060398393465546615405113181048342937527378866193236065617271782527834027295114539254186686194422346553992323083927441639598375519135597331582410569513664898531932973089637959608971084313996721237699086959330596330706323926494546371577600`

This number is decoded into our software and mathematically this is `(20*(password in hex))^e mod n` so by decrypting we get hex value as `707062c8720` which we divide by 20 to form our hex value for password which is `3838316439`

This number in plain text is `881d9` which is our password

```bash
palinux@LAPTOP-6CJCK5GG:~$ nc titan.picoctf.net 55817
*****************************************
****************THE ORACLE***************
*****************************************
what should we do for you?
E --> encrypt D --> decrypt.
e
enter text to encrypt (encoded length must be less than keysize):


encoded cleartext as Hex m: 20

ciphertext (m ^ e mod n) 3970921715843088939034957324911350626212240950470862928977787663977406608468604142079377234654007309935996972791790270166961305129444105909465676647301056

what should we do for you?
E --> encrypt D --> decrypt.
d
Enter text to decrypt: 7008823950175675948553224791235929059908363653777472741201303682989871060398393465546615405113181048342937527378866193236065617271782527834027295114539254186686194422346553992323083927441639598375519135597331582410569513664898531932973089637959608971084313996721237699086959330596330706323926494546371577600decrypted ciphertext as hex (c ^ d mod n): 707062c8720
decrypted ciphertext: ,

what should we do for you?
E --> encrypt D --> decrypt.
^C
palinux@LAPTOP-6CJCK5GG:~$
```

## OpenSSL Encrypted Secret
This secret can be uncovered using the command `openssl enc -aes-256-cbc -d -in secret.enc -k 881d9` where the `881d9` is the password of the system and we get the flag
```bash
palinux@LAPTOP-6CJCK5GG:~$ openssl enc -aes-256-cbc -d -in secret.enc -k 881d9
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
picoCTF{su((3ss_(r@ck1ng_r3@_881d93b6}palinux@LAPTOP-6CJCK5GG:~$
```

Final Flag is `picoCTF{su((3ss_(r@ck1ng_r3@_881d93b6}`
