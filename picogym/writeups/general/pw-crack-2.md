# Title
PW Crack 2

## Description
Can you crack the password to get the flag? Download the password checker here and you'll need the encrypted flag in the same directory too.

## Category
General Skills

## Points
100

## Year
2022

## Solution
After I downloaded the script and the encrypted flag, I looked at the script code first. Then, I found that the password was in hexadecimals that needed to be translated, so I just copied it and set the variable user_pw as the hex like so:
```python
def level_2_pw_check():
    user_pw = chr(0x33) + chr(0x39) + chr(0x63) + chr(0x65)
    if( user_pw == chr(0x33) + chr(0x39) + chr(0x63) + chr(0x65) ):
        print("Welcome back... your flag, user:")
        decryption = str_xor(flag_enc.decode(), user_pw)
        print(decryption)
        return
    print("That password is incorrect")
```
