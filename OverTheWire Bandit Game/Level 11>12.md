# Level 11 > 12

## Objective
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Solution
1. We have to use the `tr` command to translate character sets from one to another.
2. We also have to deshift the letters by passing the argument `'A-Za-z' 'N-ZA-Mn-za-m'`
3. `cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'`
4. Password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
