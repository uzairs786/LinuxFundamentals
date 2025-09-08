# Level 4 > 5

## Objective
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Solution
1. We use the `file` outputs the **type of file and data** a file contains
2. `file ./*`: This will list **ALL THE FILES** with the type of data they contain in the current working directory
3. The file with **ASCII Text** is human-readable. In this it is the `./-file07`
4. `cat ./-file07`
5. Password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
