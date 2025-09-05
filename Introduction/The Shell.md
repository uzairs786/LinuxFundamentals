# 🐚 Programs and Binaries

# Programs and Binaries

Commands in Linux are in-fact small programs written in a programming language
They are compiled into a format that the computer can execute, also known as a `Binary`

## So what happens if we run the `ls` command?
1. The shell reads the command
2. It searches for the `ls` program in certain directories
3. These are listed in something called the *Path environment variable*
4. After finding it, the program is executed and the directories are listed

## Path Environment Variables
- It directs the shell to the relevant directories where the command can be executed
Typing `echo $PATH`
Gives: `/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin`
'bin' just represents a binary folder


