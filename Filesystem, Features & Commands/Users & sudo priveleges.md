# 👨‍💻 User Management & Sudo Privileges

## Creating a new User
- Create User: `sudo adduser newuser`
- Set Password: `sudo passwd newuser` > prompts to type the password

## Switching Users
- `su - newuser`
- `su`: substitute user
- Verify with `whoami`

## Sudo Commands of a New User

- A new user does NOT have sudo privileges
- Any sudo command will return: `newuser is not in the sudoers file. This incident will be reported.`
- **Granting sudo privileges**:
1. Switch back ro a sudo-enabled account
2. Add user to the **sudo group**: `sudo usermod -aG newuser`
3. Revoking sudo access: `sudo deluser newuser sudo`

