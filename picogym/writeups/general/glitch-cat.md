# Title
Glitch Cat

## Description
Our flag printing service has started glitching!
$ nc saturn.picoctf.net 51109

## Category
General Skills

## Points
100

## Year
2022

## Solution
The output after connected with netcat is a string with hexadecimals in python format (chr(0x38)). Paste it into a python file and the output would be the flag.
