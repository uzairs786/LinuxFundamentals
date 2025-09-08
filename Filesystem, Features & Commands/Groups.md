# User Groups

1. **Viewing Groups**
- View all groups on the system:
`cat /etc/group`
- Each group entry lists group name, password placeholder, members etc.
- **sudo group** is the group of users that have 'root permissions'. To give a user sudo privileges, you have to add the user to the sudo group

2. **Creating a Group**
- `sudo groupadd devops`
- Verify creation: `cat /etc/group | grep devops`

3. **Adding a Group**
- `sudo usermod -aG devops newuser`
- `a`: append (do not overwrite other groups)
- `-G`: specify group
- Verify membership: `groups`

4. **Removing a User from a Group**
- `sudo gpasswd -d newuser devops`
- Verify: `su - newuser` > `groups`

5. **Deleting a Group**
- `sudo groupdel devops`
- Verify: `cat /etc/group | grep devops` > No output = devops group is deleted

6. **Adding User to Multiple Groups**
- `sudo usermod -aG admin,admin2 newuser`
- Verify: `su - newuser` > `groups` > Should show both admin1 and admin2

