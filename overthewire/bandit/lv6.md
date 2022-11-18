# Title
Bandit Level 6

## Description
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:
    human-readable
    1033 bytes in size
    not executable

## Solution
I used `find` to find the files. Since I only knew how to find the size of the files with `find`, I used that first. `find -size 1033c` yielded the answer.

Flag: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
