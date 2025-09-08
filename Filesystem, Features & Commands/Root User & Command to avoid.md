# 👑 Root User 

## Switching to Root

- Use `sudo su` to switch to the root user (superuser)
- You might be asked for your password
- `whoami` will return `root`
- `exit` will return to normal user

## ❓Why Switch to Root?

- Useful when running multiple admin commands without using `sudo` every time
- Gives unrestricted access to the system

## ❗Dangerous Command to Avoid 

`rm -rf /`

- `rm`: Remove
- `-r`: recursive (delete all directories under and contents
- `-f`: force (no confirmation prompt)
- `/`: root directory (entire file system)

## 🔒 Security & Logging

- All sudo commands are logged in `/var/log/auth.log`
- Example: to view recent sudo activity: `sudo tail /var/log/auth.log`

