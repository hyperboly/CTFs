# Title
Bandit Level 5

## Description
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Solution
ssh into the server bandit4@bandit.labs.overthewire.org at port 2220.

`cd inhere` to change working directory.

The `file` command shows the qualities of data in a file. So, `file *` should show every file. The naming schemes of these files is `-file0*` as a prefix though, so just `file *` doesn't work.

Last solution was to use the knowledge from the past bandit games and do `file ./-file0*` and the 7th file is in ASCII. `cat ./-file07` and the flag is out.

Flag: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
