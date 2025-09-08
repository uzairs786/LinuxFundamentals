# Level 13 > 14

## Objective
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

## Solution

1. We are given the file `sshkey.private` which is the private key
2. Use the `ssh` command to connect to bandit14. We use the `-i` flag to specify a private key
3. `ssh -i sshkey.private@localhost -p 2220`
4. This logs you into bandit14
5. `cd /etc/bandit_pass`
6. `cat bandit14`
7. Password: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS

