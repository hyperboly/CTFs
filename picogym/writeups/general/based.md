# Title
Based

## Description
To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337? Connect with `nc jupiter.challenges.picoctf.org 15130`.

## Category
General Skills

## Points
200

## Year
2019

## Solution
After connecting to the server, I noticed the 45s limit and also the binary. I let the time run out while searching for an online interpreter. After I got it, I inputted the result and it outputted octals. Again, I looked for an octal to ascii converter and did the process again. Last one was what I thought was base64 so I used `base64 -d` but got it wrong. I then looked again and realized it was hex. So I looked up a hex to ascii converter and finished the challenge.
