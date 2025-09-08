# Level 6 > 7

## Objective
The password for the next level is stored somewhere on the server and has all of the following properties:

`owned by user bandit7`
`owned by group bandit6`
`33 bytes in size`

## Solution
1. `find -type f -size 33c -user bandit7 -group bandit6`

We add `-user` and `-group-` to filter the user and group.

2. Password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
