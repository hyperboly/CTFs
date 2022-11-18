# Title
Bandit Level 7

## Description
The password for the next level is stored somewhere on the server and has all of the following properties:
    owned by user bandit7
    owned by group bandit6
    33 bytes in size

## Solution
I first used the `find` command to find the size of the files with 33 bytes. `find / -size 33c` would return too many files. I then had to sort by user, which I used the `-uid` option for. The uid was found with `id bandit7` which returned user(110077). So add that to the command: `find / -size 33c -uid 110077`. This still gave a ton of useless output with "permission denied."

After realizing this output was from `stderr`, just remove all the `stderr` output with `2> /dev/null`. Final command is: `find / -size 33c -uid 11007 2> /dev/null`. This gave the file `/var/lib/dpkg/info/bandit7.password`.

Flag: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
