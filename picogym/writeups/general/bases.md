# Title
Bases

## Description
What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.

## Category
General Skills

## Points
100

## Year
2019

## Route 1
I had never seen this kind of string before, so I searched up what bases are. I knew base 10, 2, 8... but not base 64. After a while, I just started testing bases such as base32.

## Solution
After trying a few bases, I found base64, which is the format the string is in. I also found the `base64` command in GNU Core Utils so I tried `echo bDNhcm5fdGgzX3IwcDM1 | base64 -d` and the flag was the output.
