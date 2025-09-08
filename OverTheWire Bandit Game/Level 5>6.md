# Level 5 > 6

## Objective

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

`human-readable`
`1033 bytes in size`
`not executable`

## Solution
1. As there are multiple subdirectories, the `find` command must be used to search and filter files.
2. `find . type f`: This lists **all files within all subdirectories under the current working directory**
3. Add `-size 1033c` as an argument and filter the size. The `c` represents the unit 'bytes'
4. Add `! -executable` to only include files that are not executable
5. Add `-exec file {} \;` to run the `file` command for each file and check what kind of file it is
6. `| grep ASCII`: Piping in the `grep` command enables you to filter the file that has human-readable text from the `file` command
7. `find . -type f -size 1033c ! -executable -exec file {} \; | grep ASCII`
8. Password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
