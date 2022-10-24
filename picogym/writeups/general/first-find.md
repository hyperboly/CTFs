# Title
First Find

## Description
Unzip this archive and find the file named 'uber-secret.txt'
    Download zip file

## Category
General Skills

## Points
100

## Year
No year

## Solution
I first downloaded the file, use `unzip` to unzip the file like `unzip file.zip`. Then, `cd` into the new directory. Using `find`, I used `find . -name "uber-secret.txt"`. Cat the file found out, and I got the flag.
