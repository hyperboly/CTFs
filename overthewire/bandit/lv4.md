# Title
Bandit Level 4

## Description
The password for the next level is stored in a hidden file in the **inhere** directory.

## Solution
ssh into the server bandit3@bandit.labs.overthewire.org at port 2220

`ls -a inhere` will show you all directories in `~/inhere`.

`cat inhere/.hidden` will show you the flag.

Flag: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
