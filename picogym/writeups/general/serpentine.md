# Title
Serpentine

## Description
Find the flag in the Python script!
Download Python script

## Category
General Skills

## Points
100

## Year
2022

## Solution
I downloaded the flag and used nvim to view and edit the flag. I found an unused `print_flag()` function in the open. Looking down, there is a boolean with displaying the flag when "b" is keyed into the program. After replacing the print line under that boolean with `print_flag()`, the flag was outputted.

```python
    if choice == 'a':
      print_encouragement()

    elif choice == 'b':
        print_flag()
```
