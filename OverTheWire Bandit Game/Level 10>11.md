# Level 10 > 11

## Objective 
The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Solution
1. We must use the `base64` command as the file is encoded in base64 data
2. As we have to decrypt the file, we must user the `-d` argument
3. `base64 -d data.txt` 
4. Password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
