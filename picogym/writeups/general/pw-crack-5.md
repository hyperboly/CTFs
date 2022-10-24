# Title
PW Crack 5

## Description
Can you crack the password to get the flag? Download the password checker here and you'll need the encrypted flag and the hash in the same directory too. Here's a dictionary with all possible passwords based on the password conventions we've seen so far.

## Category
General Skills

## Points
100

## Year
2022

## Solution
After downloading the files, I realize this script will be more complicated. I'm not good at python so I just started modifying the `level_5_pw_check()` function. First, the white space breaks the code, so use the `strip()` function for stripping out the white space. Final version:
```python
def level_5_pw_check():
    # user_pw = input("Please enter correct password for flag: ")
    for user_pw in dictionary:
        user_pw = user_pw.strip().decode("utf-8")
        user_pw_hash = hash_pw(user_pw)
        
        if( user_pw_hash == correct_pw_hash ):
            print("Welcome back... your flag, user:")
            decryption = str_xor(flag_enc.decode(), user_pw)
            print(decryption)
            return
        print("That password is incorrect")
```
