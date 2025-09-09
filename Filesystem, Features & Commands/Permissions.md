# 📁 File Permissions

File permissions control who can **read, write and execute** a file. It can be viewed using: `ls -l`
The output are as follows: `-rw-r--r--`

- `r`: Read - View file contents
- `w`: Write - Modify/edit file contents
- `x`: Execute - Run file program
- `-`: None - No Permission

## Permission Categories

`[User][Group][Others]`

- User: Owner - The person who created/owns the file
- Group: The Users belonging to the file group
- Others: Every other user on the system

## Breakdown

`-rw-r----`

- User: `-rw`: Can only read and write
- Group: `r--`: Can only read
- Others: `---`: No permissions

## Why Permissions Matter

- Control who can access, modify or run files
- Prevent unathorised access to sensitive data
- Maitain system security and stability

## Binary, Octal & String Representation of Permissions

- `rwx rw- r-x` - String
-  `111 110 101` - Binary
-  `765` - Octal

**`chmod` command is used to change permissions**

- Symbolic: `chmod u+x,g+r,o-w example.txt`: This changes the permissions of the `example.txt` file by making it `executable` for `user` (`u+x`), `readable` for `group` (`g+r`) and `removes writing access` for `others` (`u-w`)
- Numeric: `chmod 750 example.txt`: Using octal representation, we give read, write and executable access to the user (4+2+1=`7`), read and write access to the group (4+1=`5`), and no permission/access for others (`0`)

