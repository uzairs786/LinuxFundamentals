# Level 8 > 9

## Objective
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Solution
1. The `sort` file is used to take lines from a file and sort them alphabetically (A-Z, 0-9)
2. The `uniq` file removes consecutive duplicate lines from the sorted input. This means it can **only** work with the `sort` command as the `sort` command puts duplicate lines **next to each other**
3. You also have to use the `-c` argument with the `uniq` command so that it **count** the number of occurrences of the line
4. `sort data.txt | uniq -c | grep '^*1'` > This will sort the `data.txt` file alphabetically, remove the duplicate lines and have the number of occurrences next to each of them, and the `grep` with its filter will print out the line that occurs once (from the number 1)
5. Password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

