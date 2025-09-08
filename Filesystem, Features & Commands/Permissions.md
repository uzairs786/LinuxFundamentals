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

**`chmod` command is used to change permissions**
