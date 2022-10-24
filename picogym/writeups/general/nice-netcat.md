# Title
Nice netcat...

## Description
There is a nice program that you can talk to by using this command in a shell: $ nc mercury.picoctf.net 43239, but it doesn't speak English...

## Category
General Skills

## Points
15

## Year
2021

## Route 1
I looked at the output after connected to port `43239` and noticed it looks like it can be translated to ascii from some kind of encoding. The first encoding I tried was octal, but that didn't work.

## Solution
I then looked for base10 to ascii because looked like it was decimal. This outputted the flag.
