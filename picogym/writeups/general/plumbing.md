# Title
plumbing

## Description
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to jupiter.challenges.picoctf.org 14291.

## Category
General Skills

## Points
200

## Year
2019

## Solution
Upon connecting to the server, I noticed that the text just kept displaying "not the flag! not the flag!" Fairly annoying, but alright. I just connected to the server again, but piped it into grep to search for "pico."
