# Title
Big Zip

## Description
Unzip this archive and find the flag.
    Download zip file

## Category
General Skills

## Points
100

## Year
No year

## Route 1
After downloading the directory, I `unzip`ed it while grepping for "flag." This didn't work so I went into the directory and tried using `find`. The directory is too large to output anything useful.

## Solution
After looking at the hint and saw `grep`, I realized I can grep recursively. I used `grep -r "pico"` and the flag was outputted.
