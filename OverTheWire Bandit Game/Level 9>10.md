# Level 9>10

## Objective 
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Solution

Here we use the `strings` command in order to extract all the human-readable text from a **binary or non-text file**
- We use this when a file has a lot of non-printable characters
1. `strings data.txt | grep "="
2. Password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
