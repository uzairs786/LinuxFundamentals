# 🔑 Linux Commands

- These are textual commands that tell the OS what to do via the Shell
- They have various options and arguments that can modify their behaviour
- Every command has a manual which is accessed via the `man` command

`ls`: Lists all contents in current working directory

`cd`: Change directory

`pwd`: prints the current working directory

`touch`: Used to create empty files. Also used to update the timestamp of existing files. Also used to update the timestamp of existing files

`echo`: Used to display a line of text or a string that is passed as an argument. You can also redirect using this `>` the text to a new file or an existing file. You can use `>>` to overwrite the previous line.

`head` and `tail`: Used to view the beginning or end of a file. You can choose the number of line by adding `-n X`.

- `head -n 5`: This will print the first 5 lines of the file
- **Piping**: You can also choose specific lines by piping `|` > `head -n 10 myfile.txt | tail -n 5`: This will give Lines 6-10 (The last 5 lines from the top 10 lines)

`cat`: stands for concatenate. it is used to read file contents by putputing them on the terminal. Also used to combine files:

- `cat myfile1.txt myfile2.txt > combined.txt`: This combines the contents of both files into a new file (combined.txt)

It is also used to append contents to an existing file by using `>>`:

- `cat file1.txt >> file2.txt` - This would append the contents of file1.txt to file2.txt

## VIM
Vim is a powerful text editor

**Opening & Creating files**
`vim file.txt` 

- Opens `file.txt` and creates it and opens it if it doesn't exist.

**The Three Main Modes**

1. Command Mode
- Used for navigation, deleting, copying and running commands.
- Pres **Esc** to return to command mode from any other mode
2. Insert Mode
- Used for typing/editing text
- Press **i**
3. Visual Mode
- Used for selecting text visually
- Press **v**

**VIM Navigation**

- `h`: Move left
- `l`: Move right
- `j`: Move down
- `k`: Move up

- `0`: Move to the beginning of a line
- `*`: Move to end of a line
- `w`: Move word by word
- `b`: Move backwards
- `:[line number]`: Jump to a specific line
- `/example + Entr`: Search for a specific word (in insert mode). If there are multiple occurrences you can go through them by pressing `n` and `N` for previous
- `dd`: Deletes an entire line
- `D`: Deletes from cursor to end of line
- `y`: Copy (aka yank)
- `p`: Paste
- `u` Undo
- `crtl + r`: Redo
- `:syntax on`: Enable syntax highlighting
- `:set number`: Enable numbered lines
- `:set nonumber`: Disable numbered lines

## `sudo` Command

- `sudo`: super user do
- Allows a permitted user to execute commands as a root user
- Only permitted for users in the sudoers list
- Prompts for a user's own password

**When to use `sudo`?**
- Installing or Updating packages: `sudo apt install <package>`
- Editing system configuration files: `/etc/hosts`, `/etc/passwd`: It is useful when you need to `vim` into a file that is in the `/etc` folder
- Creating users, groups or managing permissions
- Any admin tasks requiring **root access**








