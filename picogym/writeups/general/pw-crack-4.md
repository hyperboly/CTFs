# Title
PW Crack 4

## Description
Can you crack the password to get the flag? Download the password checker here and you'll need the encrypted flag and the hash in the same directory too. There are 100 potential passwords with only 1 being correct. You can find these by examining the password checker script.

## Category
General Skills

## Points
100

## Year
2022

## Solution
Remove the whole function that prompts the user for a password. Replace the function with a for loop that goes through the 100 different passwords and output the flag.
```python
for user_pw in pos_pw_list:
        user_pw_hash = hash_pw(user_pw)
        
        if( user_pw_hash == correct_pw_hash ):
            print("Welcome back... your flag, user:")
            decryption = str_xor(flag_enc.decode(), user_pw)
            print(decryption)
            return
        print("That password is incorrect")
```
