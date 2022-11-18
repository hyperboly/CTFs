# Title
Bandit Level 9

## Description
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Solution
First, cat out the file and you will realize this has a million lines all looking like passwords. Then I tried the ``cat data.txt | uniq -u` command which did nothing because `man uniq` reads that repeating lines must be "adjacent" to each other. So, I had to use sort. `cat data.txt | sort | uniq -u`.
